# Javaの繰り返し処理
## rubyの繰り返しとの違い
配列から要素を取り出す繰り返しeach文⇔javaでは拡張for文を用いる

記述方法はeach文と大きく異なる
### 配列から要素を取り出す場合
```java
class Main {
  public static void main(String[] args) {
    int[] scores = {1, 5, 10};

    for(int score : scores) {
      System.out.println(score);  
    }
  }
}
```
### ArrayListから要素を取り出す場合
```java
import java.util.ArrayList;

class Main {
  public static void main(String[] args) {
    ArrayList <Integer> scores = new ArrayList <Integer>();

    scores.add(1);
    scores.add(5);
    scores.add(10);
    scores.add(15);

    for(int score : scores){
    System.out.println(score);  
    }
  }
}
```
## 拡張for文の使い方
```java
for(要素を格納する変数宣言 : 配列またはArrayListの変数名);{ //配列、ArrayListから要素を一つ取り出して要素を格納する変数に代入
取り出した要素を使用して行う処理　//代入した変数に対する処理を行う。
} //要素数分だけ処理を繰り返す
```
