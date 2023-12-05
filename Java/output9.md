# javaのメソッド続き
## アクセス修飾子
外部への公開範囲を決定する

private→同一のクラス内でのみアクセスが可能

public→どのクラスからもアクセスできる

publicにする必要がないものは極力privateにしたほうが良い
## static修飾子
メソッドを定義する際staticを付けることで静的メソッドとして実行される。

静的メソッドはクラスメソッドとも呼ばれる。
→staticを付けない場合はインスタンスメソッドとして定義される。

## メソッドの使用(引数がある場合)
```java
class Main {
  public static void main(String[] args) {
      var answer = square(5); //本引数を指定
      System.out.println(answer);
    }
  
  public static int square(int number){　//仮引数で本引数を受け取る(受け取るデータの方は指定が必要)
    return number * number;　//戻り値を返す
  }
}
```

