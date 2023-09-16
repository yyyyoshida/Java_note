# 変数

### 例：円の面積を計算するプログラム
```php
public class Greeting{
    public static void main(String[] args){
        int r;
        r = 5;
        System.out.println(r * r * 3.14);
    }
}

>> 78.5
```

### 変数を使うメリット
# 
1. 繰り返し利用できる（汎用性）
2. プログラムが読みやすくなる（可読性）
3. 後から修正がカンタン（保守性）
# 



### 変数の宣言・代入

これから扱うデータの大きさ・種類を表す
```php
     int apple;
     apple = 10
```

### 変数の初期化

**宣言・代入を同時にできる**
```php
     int apple = 10;
```
### 書き方
```php
public class Greeting{
    public static void main(String[] args){
        int num = 10;
        int apple = 15;
        System.out.println(num);
        System.out.println(apple);
    }
}

>> 10
   15
```
# 基本データ型
||型名|格納するデータ|値|利用頻度|
| ---- | ---- | ---- | ---- | ---- |
|整数|byte|だいぶ小さい整数|-128～127|△|
|整数|short|小さい整数| -32,768～32,767|△|
|整数|int|整数|-2,147,483,648～2,147,483,647|◎|
|整数|long|大きな整数|-9,223,372,036,854,775,808～9,223,372,036,854,775,807|△|
|少数|float|少数|32ビット単精度浮動小数点数|△|
|少数|double|厳密な少数|64ビット倍精度浮動小数点数|〇|
|文字|char|文字|一文字（Unicode）|〇|
|真偽値|boolean|trueかflase|true(真)かfalse(偽)|〇|
# 
- 整数はデフォルトでint型として、少数はdouble型として扱われる

　→float型の少数にはf(F)を、long型の整数にはl(L)をつける
 
- 文字のデータは''で囲む
# 
### サンプルコード
```php
public class DataType {
    public static void main(String[] args){
        int month = 12;
        int day = 29;
        float weight = 63.0f;
        double height = 168.5;
        char bloodType = 'A';

        String name = "管原";

        System.out.println("こんちにちは" + name + "です。");
        System.out.println("身長" + height + "cm、体重" + weight + "kg、");
        System.out.println("誕生日は" + month + "月" + day + "日、");
        System.out.println("血液型は" + bloodType + "型です。");
    }

>> こんにちは管原です。
   身長168.5cm、体重63.0kg、
   誕生日は12月29日、
   血液型はA型です。
```

## 参照型
```php
String name = "菅原"
```
- データ自体はメモリ上の別の場所に置かれそのアドレスの値（参照値）が変数に入る




# データ型の変換型

数値同士の演算や代入をするときに、データ型の変換が<br>　　

自動で行われる：表現できる値の幅が 小 → 大<br><br>

キャストで明示する：表現できる値のが 大 → 小<br><br><br>


```php
int i;

double d;

d = i;　　　　 //自動
       
i = (int)d;   //キャストが必要

```
### サンプルコード

```php
public class Cast {
    public static void main (String[] args) {
      int price = Integer.parseInt(args[0]);
      double rate = 0.08;         // 消費税率：８％
      int amount;

      amount = (int)(price * (1 + rate));   // rate = 2138.4 キャストして小数点を切り捨てる
      System.out.println("税金金額：" + amount + "円");
    } 
}

> java Cast 1980

>> 税金金額：2138円

```






どういう時に型変換が行われるか：例　少数の計算結果を整数に変えたいときetc..

1980円の物を買って消費税8%がついた場合の総額を計算するとき、

# 
### インクリメント・デクリメント

**値を１増加・減少させる。→ カウント用の値を更新する場面でよく使われる**
```php
public class Greeting{
    public static void main(String[] args){
        int x = 10;
        int y = 10;
        x++;
        y--;
        System.out.println("xの値:" + x);
        System.out.println("yの値:" + y);
    }
}

>> 11
   9
```


