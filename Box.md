About Vagrant Box
========

* 仮想マシンのイメージ, テンプレート．OSのディスクイメージファイル等が入ったもの．
* 仮想環境ごとに必要となる．
* ネット上に, 色んなBoxが配布されている．
* Box取得  
取得したBoxは, ~/.vagrant.d/boxes に入る．
```
$ vagrant box add <Box名> <BoxがあるURL>
```
Box名 : Boxに付けたい名前を指定(何でも良い)  
BoxがあるURL : Boxがある場所を指定

* 取得したBoxをリスト表示する
```
$ vagrant box list
```

* Box削除
```
$ vagrant box remove
```
