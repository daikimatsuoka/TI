# javaの配列
## rubyとの違い
javaの配列はrubyの配列とは異なり、最初に決めた要素数が変更できない。(要素数は最初に決めなければならない)

```java
import java.util.ArrayList;

class Main {
  public static void main(String[] args) {
   int[] scores; //配列を宣言
    scores = new int[3]; //配列の要素3つ作成し配列に代入

    scores[0] = 1;
    scores[1] = 5;
    scores[2] = 10;　//要素の値を配列に代入

    System.out.println(scores[0]);　//配列の値を取り出す
    System.out.println(scores[1]);
    System.out.println(scores[2]);
  }
}
```
