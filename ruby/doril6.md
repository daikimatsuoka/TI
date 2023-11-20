# メソッドの呼び出し
今回の場合、メソッドの呼び出し元であるget_weater_forecast("晴れ")で呼び出さなければならない。

仮引数、実引数、メソッドの呼び出し方の記憶が抜けていたので再復習

```ruby
(誤)
def get_weater_forecast(weather)
  puts "明日の天気は#{weather}です"
end

weather = "晴れ"
(正)
def get_weater_forecast(weather)
  puts "明日の天気は#{weather}です"
end

get_weater_forecast("晴れ")
