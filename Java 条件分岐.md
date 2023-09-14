# 条件分岐

### 分岐処理について

1. if文
2. 等値・関係演算子
3. if else文
4. ３つ以上の場合分け
5. swich case
# 
### if文の基本
```php
if（条件式）
　　　処理; //真の場合実行
```

### 等値・演算子
```php
public class Greeting{
    public static void main(String[] args){
        int num = 10;
        if(num == 10);
            System.out.println("10と同じです");
        if(num != 10)
            System.out.println("10と同じではないです");
    }
}

>> 10と同じです
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


