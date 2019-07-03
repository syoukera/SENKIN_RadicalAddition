# SENKIN_RadicalAddition
### 必要ファイル
|ファイル名|内容|
|:---|:---|
|driv.f|Fortran77コード，ユーザ定義|
|senkin.f|Fortran77コード，SENKINのメインルーチン（inpの読み込み，時間進行計算，ファイル出力）|
|cklib.f|Fortran77コード，cklinkの読み込み|
|dasac.f|Fortran77コード，オイラー陰解放による計算|
|inp|計算条件の設定ファイル|
|cklink|CHEMKIN interpreterで生成されるバイナリファイル，反応機構と熱力学データベースの内容が記載|
|ckout|CHEMKIN interpreterで生成されるテキストファイル，実行結果が記載|
|makefile|GNU Makeを使用してコンパイルするための設定ファイル|
### 出力ファイル
|ファイル名|内容|
|:---|:---|
|skout|結果確認用アウトプットファイル|
|terminalout|テキストファイル，ターミナル出力内容が記載|
|usrout|確認用の出力ファイル，汐除が作った|
### 使用方法
必要ファイルを準備してターミナルで以下を実行
```
$ make
```
生成されるskoutに解析結果が記載