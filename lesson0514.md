# 第2回 Programming Basics(05・13)

## Summary

Pythonの動かし方を確認してコードを書き実行する
学習したことをいかしてコンテンツをすすめる

## 教科書 独学プログラマー

### Chapter 3 プログラミング入門

#### コメント，出力，インデント，データ型，定数，変数，構文，エラー

- まず(p16-p30)読んでみよう (10分)
- 講師の実演解説
- p30までのコードを試してみよう(10分)

#### 算術演算子，比較演算子，論理演算子

- まず(p31-p38)読んでみよう (10分)
- 講師の実演解説
- p38までのコードを試してみよう(10分)

#### 条件文

- まず(p38 - p45)読んでみよう (10分)
- 講師の実演解説
- p45までのコードを試してみよう(10分)

## Paiza(CodeChronicle) & TypingClub

- [CodeChronicle](https://paiza.jp/codechronicle)のStage7まで完了させよう
- すでに完了している方や体力の回復待ちのときに[TypingClub](https://it-college.typingclub.com/)も進めよう


## 第16章Bash

最低限のLinuxコマンドを使えるようにしよう

### pwd - print name of current/working directory

現在のパス(自分がいるところ)を表示する

```
$ pwd
```

### ls - list directory contents

 指定したディレクトリ(フォルダ)のファイルとディレクトリを表示する。引数なしの場合はカレントディレクトリを表示する
 
```
$ ls /home # 絶対パス
$ ls ../   # 相対パス
$ ls ~/    # 相対パス
$ ls       # 引数なし(カレントディレクトリを表示)

```

### cd - change directory

指定したディレクトリ(フォルダ)に移動する。引数なしの場合はユーザーのHomeディレクトリへ移動

```
$ cd /home/omas # 絶対パス
$ cd ../        # 相対パス
$ cd ~/         # 相対パス(ユーザーのHomeディレクトリへ移動)
$ cd -          # 特殊(その前にいたディレクトリへ移動)
$ cd            # 引数なし(ユーザーのHomeディレクトリへ移動)
```

### mkdir - make directories

指定したディレクトリ(フォルダ)を作成

```
$ mkdir ~/foo         # home directoryにfooディレクトリを作成
$ mkdir bar buz       # current directoryに bar と buz ディレクトリを作成 
$ mkdir -p hoge/fuga  # hoge directoryの下にfuga directoryを作成
```

### rm - remove files or directories

指定したファイルまたはディレクトリを削除

```
$ rm -r ~/foo
$ rm -r foo bar
$ rm -r hoge
```

### mv - move (rename) files

(ファイル|ディレクトリ)を移動する あるいは名前を変更する

```
mv file1 file2      # file1 を file2 に変更
mv file1 dir1/      # file1 を dir1  に移動
mv file1 dir1/file2 # file1 を dir1  に file2 に変更して移動
```

### code - (VS code)

vscodeでファイルを作成する

```
$ code foo.py         # current directory に foo.py
$ code ~/foo.py       # home directory に foo.py
$ code bar.py buz.py  # bar.py buz.py を 作成
```