# オブジェクト指向

- 属性→変数：何のデータを持っているか
- 操作→メソッド：何の処理をできるか

開発効率 up 保守性 up メモリ効率 up システム化 up
# 
### 2種類のクラス
- 設計図クラス：属性と操作を記述
- 実行用クラス：mainメソッドを記述

![犬](https://min-ten.com/wp/wp-content/themes/min-ten/images/free/atom/atom3_8959.png)
![a](https://www.moringa-moringu.com/wp-content/uploads/2020/05/%E3%82%AA%E3%83%95%E3%82%99%E3%82%B7%E3%82%99%E3%82%A7%E3%82%AF%E3%83%88%E6%8C%87%E5%90%91.001-1024x576.jpeg)
![b](https://www.moringa-moringu.com/wp-content/uploads/2020/05/%E3%82%AA%E3%83%95%E3%82%99%E3%82%B7%E3%82%99%E3%82%A7%E3%82%AF%E3%83%88%E6%8C%87%E5%90%91.002-1024x433.jpeg)
# 
# 設計図クラスの書き方
**変数の定義**

例：データ型 変数名;
```php
String name;
int score;
```
**メソッドの定義**

例：戻り値の型 メソッド名(引数リスト) {
    (処理)
}
```php
void setScore(int eng, int math) {
        engScore = eng;
        mathScore = math;
```
# 
# 実行用クラスの書き方

 生成：クラス名 オブジェクト名 = new クラス名
```php
//クラス名 オブジェクト名 = new クラス名();
   Student stu1 = new Student();
```
 オブジェクト名.変数名

例：オブジェクト名・メソッド(引数)

例：オブジェクト名・メソッド(引数)
```php
stu1.name = "菅原";
stu1.setScore(80, 90);
```


# 
# 設計図クラスと実行用クラス
```php
class Student {
    //メンバ変数（属性）
    String name;     
    int engScore;
    int mathScore;
    
    //メソッド（操作）
    void display() {     
        System.out.println(name + "さん");
        System.out.println("英語" + engScore + "点・数学" + mathScore + "点");
    }
    void setScore(int eng, int math) {
        engScore = eng;
        mathScore = math;
    }
    double getAvg() {
        double avg = (engScore + mathScore) / 2.0;
        return avg;
    }    
} 
```
```php
class StuSample {
    public static void main(String[] args) {
        Student stu1 = new Student();

        stu1.name = "菅原";
        stu1.setScore(90, 80);

        stu1.display();
        System.out.println("平均" + stu1.getAvg() + "点");
    }    
}

> java StuSample

>> 菅原さん
   英語90点・数学80点
   平均85.0点
```

# サンプルコード
```php
class Car {
    //メンバ変数
    int no;
    int speed;
    
    //メソッド
    void setNo(int n) {
        no = n;
    }
    void run(int s) {
        speed = s;
    }
    void stop() {
        speed = 0;
    }
    void display() {
        System.out.println("ナンバー" + no + "速度" + speed);
    } 
}
```
```php
class DriveCar {
    public static void main(String[] args) {
        //Carクラスのオブジェクトc1を生成
        Car c1 = new Car();

        //自動者c1のナンバーを2525に設定
        c1.setNo(2525);
        //自動車c1の速度を30に設定
        c1.run(30);
        //自動車c1のナンバー、速度を表示
        c1.display();
        //自動車c1の速度を0に設定
        c1.stop();
        //自動車c1のナンバー、速度を表示
        c1.display();
    }  
}

> java DriveCar

>> ナンバー2525速度30
   ナンバー2525速度0
```


# メソッドの定義
- 引数：呼び出し元から受け取る値
- 戻り値：メソッドの処理の後に呼び出し元に返す値→return文で指定する
- 何も返さない場合は、戻り値の型→voidを記述する

# オーバーロード
クラス内に同じ名前で引数の型や数が違うメソッドを複数定義することを.オーバーロード

