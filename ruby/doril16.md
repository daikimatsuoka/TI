# クラス、インスタンスの使い方
## initializeメソッド
インスタンスが生成された際に、そのインスタンスが自動で実行する処理を記述

インスタンスに必ず実行させたい処理を記述(initializeメソッドは呼び出す必要がないため)
##　インスタンスの定義
インスタンス名 = クラス名.new(引数)　initializeメソッドに引数を渡す

## クラスメソッドの定義と呼び出し
### 定義
```ruby
def self.クラスメソッド名
end
```
### 呼び出し
クラス名.クラスメソッド名
## インスタンスメソッドの定義と呼び出し
### 定義
```ruby
def インスタンスメソッド名
end
```
### 呼び出し
インスタンス変数名.インスタンスメソッド名

```ruby
class Fruit
  def self.fresh
    puts "採れたて新鮮な果実です"
  end
 
  def initialize(name, price)
    @name = name
    @price = price
  end
 
  def introduce
    puts "#{@name}は#{@price}円です"
  end
end
 
 
apple = Fruit.new("リンゴ", 120)
orange = Fruit.new("オレンジ", 200)
strawberry = Fruit.new("イチゴ", 60)
 
Fruit.fresh
apple.introduce
orange.introduce
strawberry.introduce
