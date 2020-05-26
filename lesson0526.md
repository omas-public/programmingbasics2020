# 第7回 Programming Basics(05・26)

## Summary

演習を通してこれまでの学習を再確認する

- codingBat アカウント登録
- codingBat演習(Warmup-1)
- AOJ演習(ITPT1) 

## codingBat

### アカウント登録

1. [https://codingbat.com/python] にアクセス
2. CreateAcount
  - Email(GSuite)
  - Pass(任意)
3. prefs -> TeacherShare -> omas@std.it-college.ac.jp

### CodingBat(Python)演習

CodingBat is a free site of live coding problems to build coding skill in Java and Python.

Going through many practice problem is a great way to solidify your understanding of how the code should work.

Every big programming problem has a lot of little programming problems in it. The little programming problems have elements we see again and again -- string and list manipulation, loops, a little logic.

##### note

- Googleのページ翻訳を使用すると正しく動かないことがある

#### sleepIn

引数(weekday)が False のとき または 引数(vacation)が True の時 True を返しそれ以外は False を返す関数 sleepin を作成せよ

- [https://codingbat.com/prob/p173401]
- if文を用いて作成せよ
- ブール演算で作成せよ(if文を使わない)

#### monkey_trouble

引数(a_smile, b_smile) が ともに True または 引数(a_smile, b_smile) が ともにFalse の時 True を返しそれ以外は False を返す関数 monkey_trouble を作成せよ

- [https://codingbat.com/prob/p120546]
- if文を用いて作成せよ
- ブール演算を用いて作成せよ(if文を使わない)

#### sum_double

引数(a, b) の合計を返す関数 sum_double を作成せよ，但し a と b が等しいときは 合計を2倍にして返せ

- [https://codingbat.com/prob/p141905]
- if文を用いて作成せよ

#### diff21

引数 n と 21 の差分の絶対値を求めよ，但し n が 21 より 大きい場合は絶対値を2倍せよ

- [https://codingbat.com/prob/p197466]  
- if文を用いて作成せよ
- abs関数を用いて作成せよ abs(n) -> [https://www.google.com/search?q=python3+abs&oq=python3+abs&aqs=chrome..69i57j0l7.11013j0j9&sourceid=chrome&ie=UTF-8]

#### parrot_trouble

引数 talking が True かつ 引数 hour が 7未満 または 20以上 の時 True を返し
それ以外のときは False を返す関数 parrot_trouble を作成せよ

- [https://codingbat.com/prob/p1668841]
- if文を用いて作成せよ
- ブール演算で作成せよ(if文を使わない)

#### makes10

引数 (a, b) の いずれかが 10 または 合計が 10 の時 True を返し
それ以外は False を返す関数 makes10 を 作成せよ

- [https://codingbat.com/prob/p124984]
- if文を用いて作成せよ
- ブール演算で作成せよ(if文を使わない)


## AOJ プログラミング入門(ITP1) -> トピック #1

### 1_A Hello World 

 - [https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/1/ITP1_1_A]
 - 入力なし


### 1_B X Cubic

 - [https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/1/ITP1_1_B]
 - input 1行1列 x

入力のとり方
```
x = int(input())
```

### 1_C Rectangle

 - [https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/1/ITP1_1_C]
 - 入力 1行1列 空白で区切られた a, b

 入力のとり方
```
a, b = map(int, input().split())

# print(a, b) -> a b
```

### 1_D Watch

 - [https://onlinejudge.u-aizu.ac.jp/courses/lesson/2/ITP1/1/ITP1_1_D]
 - 入力 1行1列 S

 入力のとり方
```
S = int(input())

# Sから時間をわり出す(1時間: 60 * 60 seconds)
# Sから分をわり出す(1時間に満たない分をだす)
# Sから残りの秒をわり出す(剰余算を使う)

```
