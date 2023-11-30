# javaの条件分岐
## rubyとの違い
基本的な文法はrubyと大差ない
・条件式を()で囲む必要がある
・実行する処理を{}で囲む必要がある
・elsifではなくelse if
```java
class Main {
  public static void main(String[] args) {
    int value = 3;
    
    if (value > 0){
      System.out.println("値は正です");
    }
  }
}
```
