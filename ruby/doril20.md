# indexメソッド
indexメソッドはその文字列に対して対象の検索を開始する位置から何番目にあるかを記述する
```ruby
def count_code(str)
  puts str.index("code", 0) 
end

count_code("aaacodebbb")
