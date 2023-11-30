# 条件分岐
&& と||を複合して条件分岐を組み立てる
outside_modeがtrueという表現は==trueがなくても表現可能
```ruby
def in1to10(num, outside_mode)
  # ここに条件式を記述する
  if num >= 1 && num <= 10 || outside_mode == true
    puts "True"    
  else
    puts "False"
  end
end

# 呼び出し例
in1to10(5,false)
in1to10(11,false) 
in1to10(11,true) 
