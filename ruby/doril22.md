# 繰り返し処理とevenメソッド
eachメソッドを用いて配列の中の偶数を判定しif文を用いて配列に偶数が存在する場合はカウントを1増やすように指定する。

その判定が終わった後にcountの数を指定する。
## evenメソッド
対称の要素が偶数である場合は真を返す

```ruby
def count_evens(nums)
  count = 0
  nums.each do |num|
    if num.even?
      count += 1
    end
  end
  puts count
end
