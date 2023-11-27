# 変数について
## データの型とは
コンピュータのリソースを効率よく使うための仕組み。

配列のように値が箱に格納されて連続で並んでいるイメージ。

2進数で値が管理される。

データの種類は8種類あり扱う変数によって使う型を変更する。→int型(32bit),long型(64bit)は特に使用頻度が高い

## 静的型付け言語
javaは最初に決定した変数を変更できない仕組みとなっており、これを静的型付け言語という。

例)変数に整数を定義して文字列を代入しようとするとエラーが起こる。

## 変数宣言
javaは変数を宣言することで変数の使用が可能になる

型名　変数名; →セミコロンがないとエラーが起こる
```java
import java.util.ArrayList;

class Main {
  public static void main(String[] args) {
    int radius;
    radius = 5;
    System.out.println(radius * radius * 3.14); 
  }
}
```
## 型推論
var型を使って変数を定義することで値の種類によってデータの型が推論され、推論された型で変数が定義される。
```java
import java.util.ArrayList;

class Main {
  public static void main(String[] args) {
    var radius = 5;
    //宣言と同時に初期値を代入する場合は省略が可能
    System.out.println(radius * radius * 3.14); 

    System.out.println(((Object)radius).getClass().getSimpleName());
    //このコードで推論された型を確認できる
  }
}

```



