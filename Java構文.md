# Java 基本構文
---
#


Javaはクラスを基本に構成される
クラスは変数・関数の２つから構成される
#

### HelloWorldの出力
#
```php
class Greeting {
    public static void main(String[] args) {
        System.out.println("HelloWorld");
    }
}

>> HelloWorld
```
#
### 用語説明
#
- public：外部からアクセス可能→main関数はどこからでも利用できる

- static：staticをつけることで実体はなくても関数が使える→クラスとはデータ型であり、扱うデータの種類・大きさを決める

- void：【戻り値】終了時にどの種類のデータを返すか。main関数は戻り値を必要としない。【void:なし】

- main：関数の名前。main関数が一番のポイント

- (String[] args)：外部から投入する値
#
### main関数の処理内容
#
```php
        System.out.println("HelloWorld");
    }
}
```
#
### System.out.printlnについて
#

- System.out.println：カンタンに文字を出力するための仕組み

# 
- System：クラスの中の
- out：オブジェクトが持っている
- println：関数を使って出力









# 
### 応用？


```php
class Greeting {
    public static void main(String[] args) {
        System.out.println("Good monning");

        System.out.println("Good afternoon");

        System.out.println("Good evening");
    }
}

>> Good monning
   Good afternoon
   Good evening
```
