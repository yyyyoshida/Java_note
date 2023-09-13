# Java 文字列・数値

**文字列の出力**


```php
public class Greeting{
    public static void main(String[] args){
        System.out.println("HelloWorld");
        System.out.println("1000");
        System.out.println("1000円");
    }
}

>> HelloWorld
   1000
   1000円
```
**数値の出力**
```php
public class Greeting{
    public static void main(String[] args){
        System.out.println(10);
        System.out.println(10 + 5);
    }
}

>> 10
   15
```
**文字列と数値の組み合わせ**
```php
public class Greeting{
    public static void main(String[] args){
        System.out.println(1000 + "円");
        System.out.println("金額：" + (1000 + 500) + "円");
    }
}

>> 1000円
   金額：1500円
```
**四則演算の方法**
```php
public class Greeting{
    public static void main(String[] args){
        System.out.println(10 + 3);
        System.out.println(10 - 3);
        System.out.println(10 * 3);
        System.out.println(10 / 3);
    }
}

>> 13
   7
   30
   3   
```
**少数を扱う方法**
```php
public class Greeting{
    public static void main(String[] args){
        System.out.println(3.14 + 10);
    }
}

>> 13.14
```
