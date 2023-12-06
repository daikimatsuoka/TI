# 文字列を削除するメソッド
## sliceメソッド
配列や文字列から指定した任意の要素を削除するメソッド→！のつくメソッドを破壊的メソッドという

実引数の第一引数に文字列、第二引数に何番目の文字を削除するかを記述しmissing_charメソッドの仮引数に渡す
n番目にするとその＋1番目の文字が削除されるためsliceメソッドの削除する文字はn - 1と設定する
```ruby
def missing_char(str, n)
  str.slice!(n - 1)
  puts str
end

missing_char('kitten', 1)
```
