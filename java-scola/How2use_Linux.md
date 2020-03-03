# Linuxのつかいかた
## Linuxでは、あらゆるものがファイルで認識される。
- sda ディスクはファイルです。
- video0 カメラもファイルです。
- tty1 コマンド画面もファイルです。
- random 乱数を出力するファイルもあります。
- lp プリンターのファイルもあります。
### ファイルの場所

- フォルダは、GUIにおける視覚的な表現であり、ファイルシステム上ではディレクトリと呼ぶ。

```
/ # Root - ルート（一番うえ）
/home # 「ホーム」という名前のディレクトリ
/home/eric # ericさんのホームディレクトリ(Windowsでいうユーザーディレクトリ C:\Users\eric\ )
/home/foo/Video/secrets/Alice.mp4 # fooさんのVideoディレクトリの中のsecretsディレクトリの中のAlice.mp4
/root # rootさん（管理者）のディレクトリ
/tmp # TEMPorary テンポラリー（一時的な）ファイルを置くディレクトリ
```
- 上の表し方を絶対パスという。
- 相対的にみる。（相対パスという。）
```
# /home/foo/Images/ から Alice.mp4を参照するとき
# 今の場所（カレントディレクトリ）： ./
# 上の場所： ../
#

 ../Video/secrets/Alice.mp4

```

## コマンド

| コマンド | 意味 | 日本語で |
|----------|------|----------|
| ls  | list | 一覧 |
| cd  | change derectory | 変更 ディレクトリ |
| pwd | present working directory | 現在の作業ディレクトリ |