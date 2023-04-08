# Stack-chan_GoBottomBase

現時点で ｽﾀｯｸﾁｬﾝ を組み立てる最もシンプルな方法と思われる、[タカオさん](https://twitter.com/mongonta555)の[GoBottom版](https://mongonta.booth.pm/)のための、M5Stack本体と2個のサーボモータ、給電用のUSB TypeCコネクタがついたボードです。まるごと一式、GoBottom版のサーボ固定部分(Bracket)に収納できます。

## 他に用意するもの

- M5Stack本体 (Core BasicまたはCore2がおすすめ）
- サーボモータ2個 ([FS90MG](https://www.switch-science.com/products/8041)や[M5Stack ServoKit 180deg](https://www.switch-science.com/products/6478)、[SG90](https://akizukidenshi.com/catalog/g/gM-08761/)など)
- Groveケーブル ([M5Stack用5cm](https://www.switch-science.com/products/8664)など。すでにM5StackのUNITなどで余っているものがあればそれでもOK）
- [タカオさんの"GoBottom版"の筐体一式](https://mongonta.booth.pm/)、または[それの3Dデータ](https://github.com/meganetaaan/stack-chan/tree/dev/v1.0/case/contributed/mongonta_case_for_SG90_and_M5GoBottomBoard)を3Dプリント出力したものと必要なネジ類


## 使い方

- 筐体の組み立てなどは、[タカオさんの手順](https://raspberrypi.mongonta.com/how-to-build-easy-stackchan-m5gobottom/)を参考に行います。
- M5Stack本体と本ボードはGroveケーブルで接続します
- 2個のサーボを本ボードに接続します。ボード上の「H1」側には水平方向（足側）のサーボを、「V2」側には上下方向（筐体側）のサーボを接続します。いずれも、サーボのGND側（茶色や黒のケーブル側）を、本ボードの端側（白マークのある側）に挿し込みます。
- 本ボードを、Bracket（サーボを固定している部品）に収めます。必要に応じて両面テープやネジなどで固定してください。


## おまけ：本ボードを作りたい人は・・・

- 基板を製造します (ガーバーデータ=Stack-chan_GoBottomBase_gerber.zip)
- 部品を用意します（部品リスト=Stack-chan_GoBottomBase_BOM.csc) 主な部品は秋月電子で購入できます。USBコネクタのみ、[AliExpress](https://ja.aliexpress.com/item/1005004175942555.html)などから購入します（汎用品のようで、互換の製品が多数あります）

  - 挿入実装版（はんだ付けに自信のない方向け）: 抵抗とコンデンサはC1, C2, R3,R4を使います。
  - 表面実装版（はんだ付けに自信のある方向け）: 抵抗とコンデンサはC3, C4, R1,R2を使います。

※JLCPCBのPCBA向けのファイルは準備中です。（が、裏面に挿入実装の部品があるので、コスパが悪そうで、あまり準備する意味がないかな、と思ったり・・・）


## Author

Junichi Akita (akita@ifdl.jp, @akita11)


