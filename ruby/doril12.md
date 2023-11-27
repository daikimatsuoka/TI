# 条件分岐
範囲が狭い条件を最初に持ってくる。

(最初の処理が優先して実行されるため、複数条件が該当する場合は最初の処理が実行される)
```ruby
input = gets.to_i
if input <= 10 && input <= 0
  puts "0以下の数字です"
elsif input > 10
  puts "10より大きい数字です"
else
  puts "10以下の数字です"
end
