# 第4回 Programming Basics(05・19)

## Summary

- 先週の復習をおこなう
- Python学習に必要なUNIXコマンドを学習する
- エディタを用いてPythonプログラミングの実行を学習する

## 教科書 独学プログラマー

### Chapter 3 プログラミング入門

#### コメント

コードとして解釈しない文，Pythonでは # を用いる。
コードの理解をすすめる他，プログラミングミスの場所の特定にも用いる

#### インデント

行頭にスペースまたはタブを用いてブロックを表す，他言語と違いPythonでは必須

#### データ型

- String (文字型) 
- Integer(整数型)
- Float(小数型)
- Boolean(ブーリアン型)

#### 定数，変数

数学の定数・変数と同じ Pythonでは宣言に差はないが一般的に定数は大文字で宣言する

#### 構文エラー

文法上の間違いのこと，メッセージからエラーを特定できるように

#### 算術演算子

数学の演算子(オペレータ)のこと，記号が一部数学と異なるが計算の仕方は同じ 剰余算重要

#### 比較演算子・論理演算子

真偽値(ブーリアン)をかえす演算子，[ブール論理](https://ja.wikipedia.org/wiki/%E3%83%96%E3%83%BC%E3%83%AB%E8%AB%96%E7%90%86) 演算の順序に注意

- not (単項演算)
- and, or (2項演算)
- 論理演算の法則

#### 条件文

プログラミングの基本は 順次実行，条件分岐，繰り返しである
条件文は条件式(ブーリンアンを返す)を用いてコードをジャンプさせる

```
if ***condition*** :
    ***true part**
elif ***other condition***:
    ***true part**
elif ***other condition***:
    ***true part**
else :
    ***false part***
```

#### example

```
if True:
    print(1)

print(2)

>> 1
>> 2
```

```
if False:
    print(1)

print(2)

>> 2
```

```
if True:
    print(1)
else:
    print(2)

print(3)

>> 1
>> 3
```

```
if False:
    print(1)
else:
    print(2)
print(3)

>> 2
>> 3
```

```
if True:
    print(1)
elif True:
    print(2)
else:
    print(3)

print(4)

>> 1
>> 4
```

```
if False:
    print(1)
elif True:
    print(2)
else:
    print(3)

print(4)

>> 2
>> 4
```

```
if False:
    print(1)
elif False:
    print(2)
else:
    print(3)

print(4)

>> 3
>> 4
```

#### 2つの数字のうち大きい方を出力する

```
x = 2
y = 3

if x > y :
    print(x)
elif y > x :
    print(y)
else:
    # 同じ値の場合

```

#### 3つの数字のうち大きい方を出力する

```
x = 2
y = 3
z = 4

if x >= y:
    if x >= z:
        print(x)  # 1
    else:
        # z > x
        print(z)  # 2
else:
    # x < y
    if y > z:
        print(y)  # 3
    else:
       # z > y
       print(z)   # 4
``` 

#### 3つの数字のうち大きい方を出力する

```
x = 2
y = 3
z = 4

if x >= y and x >= z:
    print(x)
elif y >= x and y >= z:
    print(y)
else:
    print(z)
``` 

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
mv file1 dir1/file2 # file1 を file2 に変更して dir1  に 移動
```

### code - (VS code)

vscodeでファイルを作成する

```
$ code foo.py         # current directory に foo.py
$ code ~/foo.py       # home directory に foo.py
$ code bar.py buz.py  # bar.py buz.py 
```

#### exercise

1. home directory に pythonlessonというdirectoryを作る
2. pythonlesson directory で ``` $ code first.py``` 
3. 保存は ^S 