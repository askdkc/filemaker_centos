# FileMaker Server CentOS版のインストール手順
![Uploading スクリーンショット 2020-05-25 9.23.48.png…]()
## 依存パッケージ
```
yum install -y wget unzip
```

## FileMakerパッケージインストール
※rootユーザだとうまく行かない。

一般ユーザでsudoでインストールすること。
```
# sudo yum install filemaker_server-19.0.1-22.x86_64.rpm
```

## 初期パスワード設定
デフォルトの初期パスワード： admin / admin

変える時は下記コマンドで変更可能
```
fmsadmin resetpw -p 好きなパスワード -z 1234
```

## 一度再起動
```
sudo shutdown -r now
```

## Admin Consoleへアクセス
```
http://サーバのIPアドレス(or ドメイン)/admin-console/

ユーザ名：Admin
Password：リセットしたパスワード

```

