# 論理演算子と条件分岐
記述自体は正しいが、論理演算子を使うことを意識する
## aがtrueの場合にfalse、aがfalseの場合にtrue
!a

またはやかつを使う場合は()で囲む

```ruby
def police_trouble(a, b)
  if a && b || a == false && b == false
    puts "True"
  else
    puts "false"
  end
end

# 呼び出し例
police_trouble(true, true) 
police_trouble(false, false)
police_trouble(true, false)
