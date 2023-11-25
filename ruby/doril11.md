# includesメソッドの使用
今回変数strに値を代入してcheck_nameメソッド内で処理を行う。

それぞれエラーが出る処理に対してincludesメソッドを用いて条件分岐を行い、それ以外の条件では登録が完了したという処理を実行できるようにする。
## includeメソッド
特定の値や配列が含まれているかを検知する
変数.include("指定する文字列や値")
```ruby
def check_name(str) 
  if str.include?(".")
    puts "!エラー!記号は登録できません"
  elsif str.include?(" ")
    puts "!エラー!空白は登録できません"
  else
    puts "登録が完了しました"
  end
end

puts "登録したい名前を入力してください(例)YamadaTaro"
str = gets
check_name(str) 
