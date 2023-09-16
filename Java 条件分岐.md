# 条件分岐

## 構造化プログラミング

![エビフライトライアングル](https://itmanabi.com/wp-content/uploads/2018/12/seigyokozo.png)


- どちらかの処理しか実行されない
- else以降は省略
- 処理が一つの時は{ }を省略

### シンプルなif文
```php
public class Main {
    public static void main(String[] args) {
        int n = -4;

        if (n > 0) {
          System.out.println("n の値は正です");
        } else {
         System.out.println("n の値は正ではありません");
        }
    }     
}

>> n の値は正ではありません

//-------------------------------------------------------------------------------------------------------------------------------

public class Main {
    public static void main(String[] args) {
        int score = 65;

        if (score > 70) {
          System.out.println("おめでとうございます。合格です");
        } else {
          System.out.println("残念ですが不合格です");
        }
    }     
}

>> 残念ですが不合格です
```

### 一定以上の金額を値引きするif文

```php
public class Branch1 {
    public static void main (String[] args) {
        int price = Integer.parseInt(args[0]);
        double rate = 0.10;         // 消費税率：１０％
        int discount, amount;

        if( price >= 5000 ) {       // 値引き額の設定
          discount = 500;  
        } else if( price >= 3000 ) {
          discount = 300;
        } else {
          discount = 0;
        }

        amount = (int)((price - discount) * (1 + rate));
        System.out.println("値引金額：" + discount + "円");
        System.out.println("税金金額：" + amount + "円");
    }
}

> java Branch1 2999

>> 値引金額：0円
   税金金額：3298円

> java Branch1 3000

>> 値引金額：300円
   税金金額：2970円

```

### 関係演算子

**記号一覧**
|>|右辺より左辺が大きい|
|:---:|:---:|
|>=|右辺より左辺が大きい or 等しい|
|<|右辺より左辺が小さい|
|<=|右辺より左辺が小さい or 等しい|
```php
public class Greeting{
    public static void main(String[] args){
        int num = 5;
        if(num > 10)
            System.out.println("10より大きいです");
        if(num < 10)
            System.out.println("10より小さいです");
        if(num == 10)
            System.out.println("10と同じです");
    }
}

>> 10より小さいです
```


### 論理演算子

複数の条件を統合・条件を反転させるため

**２つの条件を同時に判定**

|&&|右辺・左辺が共に真|
|:---:|:---:|
|&#124;&#x7C;|右辺・左辺のどちらかが真|
|!|真偽を反転|

```php
public class Greeting{
    public static void main(String[] args){
        int num = 20;
        if(num >= 5 && num <= 10)
            System.out.println("5と10の間にあります");
        if(num < 5 || num > 10)
            System.out.println("5と10の間にありません");
    }    
}

>> 5と10の間にありません
```




