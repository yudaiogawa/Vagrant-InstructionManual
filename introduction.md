Introduction
========

#### Ⅰ．Vagrant Install
###### 〜 まずは, Vagrantをインストールしよう!! 〜
1. 公式サイトのダウンロードページから, インストーラをダウンロード．  
本稿執筆時点：vagrant_1.8.5.dmg
1. インストーラ実行．指示に従ってインストールを行う．
1. Terminalにて, [バージョン確認](Commands.md)．コマンドが動作すればOK!!  

#### Ⅱ．Hypervisor Install
###### 〜 仮想化アプリケーションをインストールしよう!! 〜
1. 本稿では, [VirtualBox](VirtualBox.md)を使用します．
1. [公式サイト](www.virtualbox.org)のDownloadsから, インストーラをダウンロード．  
本稿執筆時点：VirtualBox-5.1.2-108956-OSX.dmg
1. インストーラ実行．指示に従ってインストールを行う．

#### Ⅲ．Vagrant Box Acquisition
###### 〜 仮想マシンの元となる Box を取得しよう!! 〜
1. [Box取得](Box.md)  
ネット上から探すも良し!! 自作Excellent!! 追加しないNonsense!!  
本稿では, 公式サイトのGETTING STARTEDに沿って, 取得したいと思います．  
```
$ vagrant box add hashicorp/precise64
```
※ 選択肢が表示されるかとおもいますが, 2) virtualbox を指定．  

1. [BoxをList表示](Box.md)し, 取得したBoxが表示されればOK!!  
```
$ vagrant box list
hashicorp/precise64 (virtualbox, 1.1.0)
```

#### Ⅳ．Create [Vagrantfile](aboutVagrantfile.md)
###### 〜 仮想マシンの初期化と, 設定ファイルの作成をしよう!! 〜  
1. 仮想マシン用のディレクトリを作成し，[仮想マシン初期化](Commands.md)．  
仮想マシン毎にディレクトリの作成が必要になります．
```
$ mkdir precise64VM
$ cd precise64VM
$ vagrant init hashicorp/recise64
```

1. 初期化ができて, [Vagrantfile](aboutVagrantfile.md)が作成されたかと思います．
```
$ ls
vagrantfile
```

#### Ⅴ．Start Virtual Machine
###### 〜 かかっ仮想マシンをききっき起動させてみっみせよう/// 〜
1. Vagrantfileがあるディレクトリ内で,起動させる．
```
$ vagrant up
```

1. Virtualbox上に仮想マシンが作成されていると思います．

#### Ⅵ．Thank you
以上，凄く簡単ではありますが, 仮想マシンを起動させるまでの流れでした．  
経験もない未熟者が書いた文章ですので, ところどころにおかしいところが  
あるかもしれませんが，ご指摘等頂けたら幸いです．
