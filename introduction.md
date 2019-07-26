# Introduction

## Install Vagrant

Vagrant公式サイトを参考にインストールを行う。Vagrantのコマンドが動作すればOK。

執筆時点: `vagrant_1.8.5.dmg`

## Install Hypervisor

本稿では `VirtualBox` を使用する。VirtualBox公式サイトを参考にインストールを行う。

執筆時点: `VirtualBox-5.1.2-108956-OSX.dmg`

## Add Box

Boxの追加。

```bash
vagrant box add hashicorp/precise64
```

Boxを一覧表示し、取得したBoxが表示されればOK。

```bash
$ vagrant box list
hashicorp/precise64 (virtualbox, 1.1.0)
```

## Init

ディレクトリを作成し、初期化を行う。 `Vagrantfile` が作成されます。

```bash
mkdir precise64VM
cd precise64VM
vagrant init hashicorp/precise64
```

## Start up

`Vagrantfile` があるディレクトリ内で下記実行。仮想マシンが作成されます。VirtualBoxで確認できます。

```bash
vagrant up
```
