# Lame
Laravel + Homestead の環境を簡単に整えることを目的とするスクリプト  

## Usage
* `lame new <project_name>`  
project_nameという新規プロジェクトを作成する。
途中、/etc/hosts ファイルを編集するためにパスワードが問われます。  
ローカルでプロジェクトにアクセスするために必要な処理ですので、パスワードを入力して処理を進めてください。  

* `lame clean <project_name>`  
project_nameを削除する

* `lame --install`  
Laravel+Homesteadに必要なソフトウェアをすべてインストールする

* `lame --check`  
Laravel+Homesteadに必要な環境が揃っているかチェックする

## Ver 1.3.1
バグ修正

## Ver 1.3.0
* Homestead 5.1に対応

## 既知の不具合
・Composerが正しくインストールできない不具合。  
(対処法:Composerを別の方法で正しくインストールした場合、この不具合を回避できる）  
・SSHKeyを作成していない場合Vagrant up できない不具合  
(対処法:SSHKeyを作成する）  

これらの不具合は暇ができたら直す(｀・ω・´)ｷﾘｯ  

## インストール方法
```
$ curl -fsSL https://raw.githubusercontent.com/Kra8/lame/master/installer.sh | sh
```

### アンインストールする場合
```
$ curl -fsSL https://raw.githubusercontent.com/Kra8/lame/master/uninstaller.sh | sh
```


## 注意
このスクリプトはHomebrewを用いて必要なソフトウェアを自動でインストールします。  
そのため、Homebrewをインストールしていない環境ではHomebrewを最初にインストールします。  
その他インストールするソフトウェアはLaravel及びHomesteadの動作に必要なものです。  
すでに、必要なソフトウェアがインストールされている場合はインストールされません。  

## インストールされるソフトウェア
* Homebrew
* VirtualBox
* Vagrant
* Composer
* Laravel
* Homestead

## LICENSE
[The MIT License (MIT)](https://github.com/Kra8/Lame/blob/master/LICENCE)

## 動作環境
macOS - OSX El Capitan 10.11.x 以上  
php5.6 以上  



@version    1.3.1
@update     2017/04/22  
@develop    K.Asai (asai@teaapplications.com)  
