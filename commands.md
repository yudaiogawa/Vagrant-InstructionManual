# Commands

[Documentation - Commands(CLI)](https://www.vagrantup.com/docs/cli/)

## Init

- 初期化

```bash
vagrant init [box name(optional)] [url(optional)]
```

## Box

- Boxの追加

```bash
vagrant box add [name(optional)] [address]
```

- インストールされているBoxの一覧表示

```bash
vagrant box list
```

## Up

- ゲストマシーン作成および起動

```bash
vagrant up
```

## SSH

- ゲストマシーンへの接続

```bash
vagrant ssh
```

## Status

- Vagrantが管理しているマシーンの状態を確認する

```bash
vagrant status
```

## Halt

- 稼働中のゲストマシーンを停止する

```bash
vagrant halt
```

## Reload

- ゲストマシーンの再起動

```bash
vagrant reload
```

## Suspend

- バーチャルマシーンをスリープ状態にする

```bash
vagrant suspend
```

## Resume

- スリープ状態からの復帰

```bash
vagrant resume
```

## Destroy

- ゲストマシーンの削除

```bash
vagrant destroy
```
