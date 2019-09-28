<h1 align="center">Commands</h1>
<br>

[Documentation - Commands(CLI)](https://www.vagrantup.com/docs/cli/)

<br>

### Init

- 初期化

```bash
$ vagrant init [box name(optional)] [url(optional)]
```

<br>

### Box

- Boxの追加

```bash
$ vagrant box add [name(optional)] [address]
```

- インストールされているBoxの一覧表示

```bash
$ vagrant box list
```

<br>

### Up

- ゲストマシーン作成および起動

```bash
$ vagrant up
```

<br>

### SSH

- ゲストマシーンへの接続

```bash
$ vagrant ssh
```

<br>

### Status

- Vagrantが管理しているマシーンの状態を確認する

```bash
$ vagrant status
```

<br>

### Halt

- 稼働中のゲストマシーンを停止する

```bash
$ vagrant halt
```

<br>

### Reload

- ゲストマシーンの再起動

```bash
$ vagrant reload
```

<br>

### Suspend

- バーチャルマシーンをスリープ状態にする

```bash
$ vagrant suspend
```

<br>

### Resume

- スリープ状態からの復帰

```bash
$ vagrant resume
```

<br>

### Destroy

- ゲストマシーンの削除

```bash
$ vagrant destroy
```
