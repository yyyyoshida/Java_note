# 配列

配列は同じデータ型の変数を複数まとめて管理するもの<br>
配列の生成には new を使う。生成時にデフォルト初期値が設定される<br><br>

**初期値早見表**
|整数|型|デフォルト値|
| ---- | ---- | ---- |
|整数|byte|0|
|整数|short|0|
|整数|int|0|
|整数|long|0|
|浮動小数点数|float|0.0|
|浮動小数点数|double|0.0|
|文字|char|\u0000|
|真偽値|boolean|false|
|参照型|String|null|

### サンプルコード
```php
public class Array {
    public static void main(String[] args){
        int[] score = new int[4];
        score[0] = 80;
        score[1] = 100;
        score[2] = 70;

        String[] name = {"菅原", "村山", "寺島", "のび太"};

        System.out.println(name[0] + "さん：" + score[0] + "点数");
        System.out.println(name[1] + "さん：" + score[1] + "点数");
        System.out.println(name[2] + "さん：" + score[2] + "点数");
        System.out.println(name[3] + "さん：" + score[3] + "点数");
        System.out.println("受験者：" + score.length + "名");
    }
}

>> 菅原さん：80点数
   村山さん：100点数
   寺島さん：70点数
   のび太さん：0点数
   受験者：4名
```
補足：それぞれ同じ
```php
int[] score = new int[3];
        score[0] = 80;
        score[1] = 100;
        score[2] = 70;


int[] score = {80, 100, 70};
```
# 多次元配列

配列の配列が作れる

![エビフライトライアングル](https://i0.wp.com/it-level-up.club/wp-content/uploads/2017/09/array3.gif)

### サンプルコード
```php
public class MultiArray {
    public static void main(String[] args){
        int[][] allScore = new int[2][3];
        allScore[0][0] = 80;
        allScore[0][1] = 100;
        allScore[0][2] = 75;
        allScore[1][0] = 85;
        allScore[1][1] = 95;
        allScore[1][2] = 80;

        // 多次元配列の初期化
        // int[][] allScore = {{10, 20 ,30}, {40, 50, 60}};

        System.out.println(allScore[0][0] + "点数");
        System.out.println(allScore[0][1] + "点数");
        System.out.println(allScore[0][2] + "点数");
        System.out.println(allScore[1][0] + "点数");
        System.out.println(allScore[1][1] + "点数");
        System.out.println(allScore[1][2] + "点数");

        System.out.println("allScore.lenght:" + allScore.length);
        System.out.println("allScore[0].lenght:" + allScore[0].length);
    } 
}

>> 80点数
   100点数
   75点数
   85点数
   95点数
   80点数
   allScore.lenght:2
   allScore[0].lenght:3
```
