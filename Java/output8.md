# javaのメソッド
## mainメソッド
### ファイルを実行するとメインメソッドが実行される

mainメソッドの引数は必ず決められたように記載

javaのmainメソッドはファイルの実行時に自動的に実行されるため、mainメソッドを実行するコードを書かなくても実行される。
### メインメソッドの引数は必ず決められたとおりに記載する
データの方等を￥変更するとエラーが出てしまうため必ず提携通りに記述する
## メソッドの使い方
```java
アクセス修飾子 static修飾子 返り値のデータ型　メソッド名() {
  // 行いたい処理
}
```
```java
class Main {
  public static void main(String[] args) {
    sayHello();
    }
  
  public static void sayHello() {
    System.out.println("Hello World");
    return;
  }
}
```
### rubyとの違い
返り血のデータの方を指定する必要がある

引数がないメソッドでも括弧省略ができない

def endの代わりに波括弧で囲む
