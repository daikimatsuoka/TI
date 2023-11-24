# 配列の取り出しとeach_with_index
配列から任意の数字を取り出して何番目にあるか調べたい。
今回、仮引数target_numとinputに存在するnumが等しければ処理を実行できるようにする。

また、そのnumが配列に存在する場合input+1番目にあるという処理を記述。(＋1をしないと0から始まってしまう)
## each_with_index
配列名.each_with_index do |item, i|(そのアイテムがi＋1番目にある)
```ruby
def search(target_num, input)
  # 処理を記述
  input.each_with_index do |num, index|
    if num == target_num
      puts "#{index + 1}番目にあります"
      return
    end
  end
  puts "その数は含まれていません"
  
end

input = [3, 5, 9 ,12, 15, 21, 29, 35, 42, 51, 62, 78, 81, 87, 92, 93]
# 呼び出し例
search(3, input)
