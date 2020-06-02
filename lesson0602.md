# 第10回 Programming Basics(06・02)

## Summary

本日学習するループでプログラミングの基礎は終了する。
ここまでの知識でCodingBat,AOJ,Paizaの殆どの問題を解くことができる
演習問題を数多くこなすことでプログラムでの解決方法が身につく

プログラムが難しいと感じている諸君は以下を熟読すること

- コードを写経する時，予測しているか(これを変化させるとこうなる)
- プログラムを書く前に手順をその問題が解けるか(例 縦3cm 横2cmの4角形の面積)
- 問題を解くのに必要な手順を考えているか(あれをやって次にこれをやって)
- 大きな問題に含まれる小さな問題をプログラミングできるか(例 平均を出す，一番大きい数を求める)
- 時間を無駄にしていないか(一定時間以上やってもできなければ他の解決を考える)

学習が進んでいる諸君はどんどん演習を進めてもらいたい, 使い方をもう一度確認する

- [AOJ exercise](https://github.com/omas-public/AOJ2)
- [Codingbat exercise](https://github.com/omas-public/codingbat)

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

### front_times

引数(str)の最初の3文字を 引数(n)回コピーした文字列を作成して返せ
ただしstrが3文字未満ならそのまま返せ

- [https://codingbat.com/prob/p165097]
- 文字列のスライス
- 文字列の掛け算
- 文字列の長さ

### string_bits

引数(str)の偶数番目の文字を取り出して合成した文字列を返せ

- [https://codingbat.com/prob/p113152]
- 文字列のスライス(第3引数)

## 教科書 独学プログラマ

### Chapter7 ループ (p104)

while Loop, for Loop, range, enumerate の使い方を憶えよう


- 講師実演解説
- (p88-p102) を読んでみよう (15分)
- コードを試してみよう (30分)

