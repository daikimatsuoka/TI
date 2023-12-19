# 条件分岐
talkingが真の場合、20時以降と7時以前をどう表現するかがポイント

talkingが真はtalkingのみの記載で表現できる

```ruby
def parrot_trouble(talking, hour)
  if (talking == true) && (hour < 7 || hour > 20)
    puts "NG"
  else 
    puts "OK"
  end
end

parrot_trouble(true, 8)
