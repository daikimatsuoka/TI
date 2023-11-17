# メソッドの使い方
メソッドないでメソッド外の変数を用いるには引数を使用する
## エラーの原因
メソッド外で定義した変数を引数を用いずにメソッド内で使用していたためエラーが起きた(スコープの概念)

```ruby
price = 300

def calculate_price_with_tax(price)
  tax = 0.1
  return price + price * tax
end

calculate_price_with_tax(price)
