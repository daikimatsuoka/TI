## 繰り返し処理
表示する回数をgets.to_iをもちいてユーザーに入力させ引数を用いてメソッド内で使用。

メソッド内で引数に対して繰り返し処理を行うことで表示させる文字を繰り返し表現する

```ruby
def output(num)
  num.times do
    puts "Hello!"
  end
end

puts "何回表示させますか？"

num = gets.to_i

output(num)
