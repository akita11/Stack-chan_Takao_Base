# Stack-chan_Takao_Base

現時点で ｽﾀｯｸﾁｬﾝ を組み立てる最もシンプルな方法と思われる、[タカオさん](https://twitter.com/mongonta555)の[タカオ版（旧称：GoBottom版）](https://mongonta.booth.pm/)のための、M5Stack本体と2個のサーボモータ、給電用のUSB TypeCコネクタがついたボードです。電源スイッチもついています。まるごと一式、タカオ版のサーボ固定部分(Bracket)に収納できます。市販のUSB Type-CコネクタつきのACアダプタ等をつないで給電して使用します。以下のように、本体の後ろ側からUSB Type-Cケーブルで給電して動作させることができます。

<img src="https://github.com/akita11/Stack-chan_Takao_Base/blob/main/usage1.jpg" width="240px">

<img src="https://github.com/akita11/Stack-chan_Takao_Base/blob/main/usage1.jpg" width="240px">

<img src="https://github.com/akita11/Stack-chan_Takao_Base/blob/main/usage1.jpg" width="240px">


## 表面実装部品版

※[完成品としてスイッチサイエンスで委託販売中](https://www.switch-science.com/products/8905)です

<img src="https://github.com/akita11/Stack-chan_Takao_Base/blob/main/boardB-1.jpg" width="240px">

<img src="https://github.com/akita11/Stack-chan_Takao_Base/blob/main/boardB-2.jpg" width="240px">

## 挿入実装部品版

※[部品キットとしてスイッチサイエンスで委託販売中](https://www.switch-science.com/products/8906)です

<img src="https://github.com/akita11/Stack-chan_Takao_Base/blob/main/boardA-1.jpg" width="240px">

<img src="https://github.com/akita11/Stack-chan_Takao_Base/blob/main/boardA-2.jpg" width="240px">

※部品キット版では、[作り方](https://github.com/akita11/Stack-chan_Takao_Base/blob/main/Build/README.md)の手順で部品をはんだ付けしてください。


## 他に用意するもの

- M5Stack本体 (Core BasicまたはCore2がおすすめ）
- サーボモータ2個 ([FS90MG](https://www.switch-science.com/products/8041)や[M5Stack ServoKit 180deg](https://www.switch-science.com/products/6478)、[SG90](https://akizukidenshi.com/catalog/g/gM-08761/)など)
- Groveケーブル ([M5Stack用5cm](https://www.switch-science.com/products/8664)など。すでにM5StackのUNITなどで余っているものがあればそれでもOK）
- ["タカオ版（旧称：GoBottom版）"の筐体一式](https://mongonta.booth.pm/)、または[それの3Dデータ](https://github.com/meganetaaan/stack-chan/tree/dev/v1.0/case/contributed/mongonta_case_for_SG90_and_M5GoBottomBoard)を3Dプリント出力したものと必要なネジ類


## 使い方

- 筐体の組み立てなどは、[タカオさんの手順](https://raspberrypi.mongonta.com/how-to-build-easy-stackchan-m5gobottom/)を参考に行います。
- M5Stack本体と本ボードはGroveケーブルで接続します
- 2個のサーボを本ボードに接続します。ボード上の「H1」側には水平方向（足側）のサーボを、「V2」側には上下方向（筐体側）のサーボを接続します。いずれも、サーボのGND側（茶色や黒のケーブル側）を、本ボードの端側（白マークのある側）に挿し込みます。
- 本ボードを、Bracket（サーボを固定している部品）に収めます。必要に応じて両面テープやネジなどで固定してください。


## うまく動作しないときは・・・

「バッテリをはずしたCore2にこのボードとサーボを接続し、Core2側にUSBケーブルをつないでプログラムの書き込みを行う」場合に、Core2が起動しない、またはリセット・再起動を繰り返す、という現象があるようです。その場合は、いったんGroveケーブルをはずしてCore2単体でプログラムを書き込んでから、このボードのUSBコネクタ（本体背面）から電源を供給して使用してください。


## おまけ：本ボードを作りたい人は・・・

- 基板を製造します (ガーバーデータ=Stack-chan_Takao_Base_gerber.zip)
- 部品を用意します（部品リスト=Stack-chan_Takao_Base_BOM.csv) 主な部品は秋月電子で購入できます。USBコネクタのみ、[AliExpress](https://ja.aliexpress.com/item/1005004175942555.html)などから購入します（汎用品のようで、互換の製品が多数あります）

  - 挿入実装版（はんだ付けに自信のない方向け）: 抵抗とコンデンサはC1, C2, R3,R4を使います。
  - 表面実装版（はんだ付けに自信のある方向け）: 抵抗とコンデンサはC3, C4, R1,R2を使います。

## Author

Junichi Akita (akita@ifdl.jp, @akita11)


