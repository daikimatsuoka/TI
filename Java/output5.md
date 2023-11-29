# javaのリスト
rubyの配列と似たデータ管理の仕組み

要素を順序づけて管理する。

要素を事後的に追加したり削除できる。

## ArrayList
可変長配列→要素数を変更できるための配列を使うための仕組み
### 記述方法
```java
import java.util.ArrayList; //ライブラリをインポートする(開発環境を利用すると自動的に補完できる)

class Main {
  public static void main(String[] args) {
  ArrayList<Integer> scores = new ArrayList<Integer>();　//ArrayListの宣言

    scores.add(1);
    scores.add(5);
    scores.add(10);
    scores.add(15);　//値の代入(addメソッドを利用すると要素はArrayListの末尾に追加)

    System.out.println(scores.get(0));
    System.out.println(scores.get(1));
    System.out.println(scores.get(2));
    System.out.println(scores.get(3));　//getメソッドを用いてArrayListのとリだしを行う
  }
}
```
