# 条件分岐
条件分岐は寄り細かい条件を最初に持ってくる。

(最初の処理が優先して実行されるため)
```ruby
input = gets.to_i
if input <= 10 && input <= 0
  puts "0以下の数字です"
elsif input > 10
  puts "10より大きい数字です"
else
  puts "10以下の数字です"
end
