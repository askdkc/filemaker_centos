# FileMaker CentOSへのインストール

## 依存パッケージ
```
yum install -y aide aspell avahi cyrus-sasl* gdb httpd \
ImageMagick java-1.8.0-openjdk libevent libXpm libvpx \
 mod_ssl mysql-connector-odbc ntp redhat-lsb-core scl-utils \
t1lib unixODBC yum-utils unzip zip baekmuk-ttf-batang-fonts \
ipa-pgothic-fonts liberation-fonts-common \
liberation-mono-fonts liberation-sans-fonts \
wqy-microhei-fonts wqy-zenhei-fonts
```

## もしかすると以下だけで行けるかも
```
yum install wget
yum install unzip
```

## FileMakerパッケージインストール
rootユーザだとうまく行かない。一般ユーザでsudoでインストールすること。
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

