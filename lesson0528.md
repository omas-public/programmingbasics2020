# 第9回 Programming Basics(05・28)

## Summary

- AOJ演習(Topic 2)を行う
- コンテナ，文字列の扱いを学習する(教科書 Chapter 5,6)
- CodingBatで文字列の演習を行う


## 教科書 独学プログラマ

### Chapter5 コンテナ (p70)

コンテナとは複数の値を保持できるデータ構造である。list, tupple, dict はコンテナである。それぞれのコンテナの作り方と値の参照の仕方を学習する。

#### list, tupple, dict manipulate
```
# create
fluit_list = ['apple', 'orange', 'peer']
fluit_tupple = ('apple', 'orange', 'peer')
fluit_dict = {'apple':'りんご', 'orange':'みかん', 'peer':'なし'}

# fetch
fluit_list[index]   # fluit_list[0] => 'apple'
fluit_tupple[index] # fluit_tupple[1] => 'orange'
fluit_dict[key]     # fluit_dict['peer'] => 'なし'

# exception
fluit_list[3]   # out of range
fluit_tupple[3] # out of range
fluit_dict['grape'] # key error

# include, exclude
'apple' in fluit_list     # True (include)
'grape' in fluit_tupple   # False (exclude)
'grape' not in fluit_dict # True (exclude)

# append
fluit_list.append('grape')    # ['apple', 'orange', 'peer', 'grape']
fluit_dict['grape'] = 'ぶどう' # {'apple':'りんご', 'orange':'みかん', 'peer':'なし', 'grape': 'ぶどう'}

# delete
fluit = fluit_list.pop() # fluit => 'grape' , fluit_list => ['apple', 'orange', 'peer']
del fluit_dict['grape']  # fluit_dict => {'apple':'りんご', 'orange':'みかん', 'peer':'なし'}

# modify
fluit_list[0] = 'apple1'        # fluit_list[0] => 'apple1'
fluit_dict['apple'] = 'りんご1'  # fluit_dict['apple'] => 'りんご1'

```

### Chapter6 文字列操作 (p88)

文字列は文字のタプルと考えよ "abc" => ('a','b','c') よって参照のしかたは同じである，逆にこれから学習するスライスはタプルやリストに応用できる。

文字列が持っているメソッド(split, join, replace,index)を憶えよう

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
