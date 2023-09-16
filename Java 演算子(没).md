# 算術演算子
Config files for my GitHub profile.
|演算子|概要|例|
| ---- | ---- | ---- |
|+|加算|1 + 2 > 3|
|-|減算|5 – 2 > 3|
|*|乗算|3 * 4 > 12|
|/|除算|5.0 / 2 > 2.5|
|%|剰余|5 % 2 > 1|
|+|文字の連結|"A" + "B" > AB|
|++|インクリメント|x = 1;x++; > 2|
|--|デクリメント|1;x- -; > 0|



### インクリメント／デクリメント演算子

**a++ → aに1を加える、a = a + 1 、a += 1 と同じ**

**書き方**
```php
    int x = 1;
    int y = x++;
    System.out.println(y);

>> 1

    int x = 1;
    int y = ++x;
    System.out.println(y);

>> 2
```

**算術演算子サンプルコード**
```php
public class Operator {
    public static void main(String[] args){
        int a = Integer.parseInt(args[0]);
        int b = Integer.parseInt(args[1]);

        System.out.println("a = " + a + ", b = " + b);
        System.out.println("a + b = " + (a + b));
        System.out.println("a - b = " + (a - b));
        System.out.println("a * b = " + (a * b));
        System.out.println("a / b = " + (a / b));
        System.out.println("a % b = " + (a % b));
        System.out.println("a >= b = " + (a >= 0));
        System.out.println("(a >= 0 && (b >= 0) :" + ((a >= 0) && (b >= 0)));
    }    
}　　　//コンパイル値 7 2

>> a + b = 9
   a - b = 5
   a * b = 14
   a / b = 3
   a % b = 1
   a >= b = true
   (a >= 0 && (b >= 0) :true

```




