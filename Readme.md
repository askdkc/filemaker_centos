# FileMaker CentOSへのインストール

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
```
fmsadmin resetpw -p 好きなパスワード -z 1234
```

## Admin Consoleへアクセス
```
http://IP_ADDR/admin-console/

ユーザ名：Admin
Password：リセットしたパスワード

```

