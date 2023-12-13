# scanメソッド
引数で指定した文字を数え、配列として返す

配列の数を数えたいためlengthを用いる

```ruby
def count_hi(str)
  puts str.scan("hi").length
end

count_hi('abc hi hohihihihi')
