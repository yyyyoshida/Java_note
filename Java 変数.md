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


### int：データ型

**変数の宣言・代入**

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
### データ型について
#
**代表的なデータ型**

1. データ型６種類
2. データ型の大きさ
3. データの種類（整数・実数）
# 

### データ型大きさ・種類

||大きさ| 種類 |
|:---:|:----:|:-----:|
|char|１バイト|文字|
|short|２バイト|整数|
|int|４バイト|整数|
|long|８バイト|整数|
|float|４バイト|少数|
|double|８バイト|少数|

**よく使うのは３つだけ**

char・int・double

### doubleとintの変換 （キャストについて）

データ型を強制的に変換する仕組み

例： 少数 → 整数、 整数 → 少数

### キャスト方法

```php
public class Greeting{
    public static void main(String[] args){
        double pi = 3.14;
        System.out.println((int)pi);
    }
}

>> 3
```

### 複合代入演算子

変数の値を変数それ自体の値を使って更新 → 値を更新する場面でよく使われる**

**xそれ自体の値を５増やす**
```php
     int x = 10;
     x = x + 5;

// シンプルに更新ができる

     int x = 10;
     x += 5;
```

**例**
```php
public class Greeting{
    public static void main(String[] args){
        int apple = 10;
        apple += 5;
        System.out.println(apple);
    }
}

>> 15
```
### インクリメント・デクリメント

**値を１増加・減少させる。→ カウント用の値を更新する場面でよく使われる**
```ph
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

