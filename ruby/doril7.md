# Dateクラスの使い方
取得した今日の曜日の使い方に問題あり

正しくは#{配列.変数}

また、イコールの表現にも誤りがあった(確認ミス)。正しくは==
```ruby
（誤）
require "date"

day = Date.today.wday

week_day = ["日曜日","月曜日","火曜日","水曜日","木曜日","金曜日","土曜日"]

if day = 5
  puts "今日は金曜日だ！！！"
else
  puts "今日は#{week_day.day}"
end

（正）
require "date"

day = Date.today.wday

week_day = ["日曜日","月曜日","火曜日","水曜日","木曜日","金曜日","土曜日"]

if day == 5
  puts "今日は金曜日だ！！！"
else
  puts "今日は#{week_day[day]}"
end
