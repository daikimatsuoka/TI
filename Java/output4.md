# javaの配列
## rubyとの違い
javaの配列はrubyの配列とは異なり、最初に決めた要素数が変更できない。(要素数は最初に決めなければならない)
## 記述方法
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
## 様々な配列の記述方法
### 宣言と代入は同時に行うことが可能
```java
int[] scores = new int[3];
```
### 型推論による宣言も可能
```java
var[] scores = new int[3];
```
### 宣言から代入までを同時で行う
```java
int scores[] = {1, 5, 10};
// 宣言時に代入する値が確定していなければ使用できない
```
