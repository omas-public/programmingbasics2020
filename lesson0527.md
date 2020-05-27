# 第8回 Programming Basics(05・27)

## Summary

- AOJ演習(Topic 2)を行う
- コンテナ，文字列の扱いを学習する(教科書 Chapter 5,6)
- CodingBatで文字列の演習を行う


## AOJ プログラミング入門(ITP1) -> トピック #2

### ITP1_2_A Small, Large, or Equal

 - [https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/2/ITP1_2_A]
 - input 1行1列 a, b
 - 2つの引数(a, b)をとり a が b 未満なら True を返す関数 small を作成して使用せよ
 - 2つの引数(a, b)をとり a が b より大きいなら True を返す関数 large を作成して使用せよ
 - 2つの引数(a, b)をとり a と b 等しいなら True を返す関数 equal を作成して使用せよ

 入力のとり方

```
a, b = map(int, input().split())
```

### ITP1_2_B Range

 - [https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/2/ITP1_2_B]
 - input 1行1列 a, b, c
 - a が b未満ならTrueを返す関数 lessthan(a, b) を作成してみる

入力のとり方

```
a, b, c = map(int, input().split())
```

###  ITP1_2_C Sorting Three Numbers

 - [https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/1/ITP1_2_C]
 - 入力 1行1列 空白で区切られた a, b, c
 - a が b以下の時 True を返す関数 lessthan_or_equal(a, b)を作成してみる

 入力のとり方
```
a, b, c = map(int, input().split())

# 順列を考える a <= b <=c, a <= c <=b ...
# 3P3 => 3! => 6通り

```

### ITP1_2_D Circle in a Rectangle

 - [https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/1/ITP2_1_D]
 - 入力 1行1列 W, H, x, y, r

 入力のとり方
```
 W, H, x, y, r = map(int, (input().split())

# x - r(円の左端)，x + r(円の右端) ，y + r ....

```

## CodingBat(Python)演習

### near_hundred

intの引数(n)と100または200の差分の絶対値が10以内なら Trueを返しそれ以外は　False を返す関数 near_hundred を作成せよ

- [https://codingbat.com/prob/p124676]
- if文を用いて作成せよ
- ブール演算で作成せよ(if文を使わない)

### pos_neg

intの引数(a, b)の一方が正の数(Positive)，もう片方の数が負の数(Negative)のときに True を返す関数 pos_neg を作成せよ。
但し 引数 negative が True のときは a,b がともに 負の数(Negative)のときだけ True を返せ

- [https://codingbat.com/prob/p124676]
- if文を用いて作成せよ


## 教科書 独学プログラマ

### Chapter5 コンテナ (p70)

- 講師実演解説
- (p70-p87) を読んでみよう (15分)
- コードを試してみよう (30分)

### Chapter6 文字列操作 (p88)

- 講師実演解説
- (p88-p102) を読んでみよう (15分)
- コードを試してみよう (30分)

## CodingBat(Python)文字列演習

### not_string

stringの引数(str) が 'not' で開始していない場合は
先頭に 'not ' を付け加えて返せ
それ以外のときはそのまま引数を返せ

- [https://codingbat.com/prob/p189441]
- if文 と 文字列のスライスを使用せよ

### missing_char

空ではないstringの引数(str) と intの引数(n)が与えられる
str の n 番目の文字を削除した 文字列を返せ
- [https://codingbat.com/prob/p149524]
- 文字列のスライスを使用してindexの前と後ろの文字を取り出し合成

### front_back

stringの引数(str) の 最初の文字と最後の文字を交換した文字列を作成して返せ

- [https://codingbat.com/prob/p153599]
- 文字列のスライスを使用して一文字めと最後の文字を取り出す

### front3

stringの引数(str)の先頭3文字を取り出し，3回コピーした文字列を作成して返せ，但しstrが3文字未満ならそのまま返せ

- [https://codingbat.com/prob/p147920]
- 文字列のスライスを使用，if文で判定
