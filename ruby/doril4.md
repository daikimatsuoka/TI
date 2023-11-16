# クラス、インスタンス
## インスタンスの生成
article = Article.new()←引数を指定

指定した実引数をinitializeメソッドの仮引数に受け渡す

## initializeメソッド
initializeメソッドを用いることで、インスタンスを呼び出す動作を省くことができる。

その後インスタンス変数の値を返すための専用のメソッドを定義

```ruby
class Article

  def initialize(author, title, content)
    @author = author
    @title = title
    @content = content
  end

  def author
    @author
  end

  def title
    @title
  end

  def content
    @content
  end

end

article = Article.new("阿部", "Rubyの素晴らしさについて", "Awesome Ruby!")

puts "著者: #{article.author}"
puts "タイトル: #{article.title}"
puts "本文: #{article.content}"
