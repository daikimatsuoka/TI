# unless構文の使い方
unlessの条件式がfalseの場合に処理を実行する。

今回の場合　a + b が0以下の場合がfalseであるためそのように記述する

```ruby
a = 3
b = 4

unless a + b <= 0
  puts "計算結果は0より大きいです"
end

