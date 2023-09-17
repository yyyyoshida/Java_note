# オブジェクト指向

![犬](https://min-ten.com/wp/wp-content/themes/min-ten/images/free/atom/atom3_8959.png)
![a](https://www.moringa-moringu.com/wp-content/uploads/2020/05/%E3%82%AA%E3%83%95%E3%82%99%E3%82%B7%E3%82%99%E3%82%A7%E3%82%AF%E3%83%88%E6%8C%87%E5%90%91.001-1024x576.jpeg)
![b](https://www.moringa-moringu.com/wp-content/uploads/2020/05/%E3%82%AA%E3%83%95%E3%82%99%E3%82%B7%E3%82%99%E3%82%A7%E3%82%AF%E3%83%88%E6%8C%87%E5%90%91.002-1024x433.jpeg)
- 属性→変数：何のデータを持っているか
- 操作→メソッド：何の処理をできるか

開発効率 up 保守性 up メモリ効率 up システム化 up
# 
### 2種類のクラス
- 実行用クラス：mainメソッドを記述
- 設計図クラス：属性と操作を記述

### 設計図クラス(属性)
```php
 class Student {
    String name;     //メンバ変数（属性）
    int engScore;
    int mathScore;

    /*void display() {     //メソッド（操作）
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
}*/
```
# メソッドの定義
- 引数：呼び出し元から受け取る値
- 戻り値：メソッドの処理の後に呼び出し元に返す値→return文で指定する
- 何も返さない場合は、戻り値の型→voidを記述する

# 簡易サンプル

### 引数なし、戻り値なし

```php
main(～) {
  .
  .
display();
```

```php
void display() {
  System.out.println(name);
   .
   .
}
```
### 引数あり、戻り値なし
```php
setScore(90, 80);
```
```php
void setScore(int eng, int math)
  engScore = eng;
  mathScore = math;
}
```
### 引数なし、戻り値あり
```php
getAvg();    //戻り値85.0
```
```php
double getAvg() {
  double avg = (engScore + mathScore) / 20;
  return avg;
}
```
メソッドサンプル
```php
 class Student {
    /*String name;     //メンバ変数（属性）
    int engScore;
    int mathScore;*/

    void display() {     //メソッド（操作）
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

### オブジェクトの使い方
**①生成**

クラス名　オブジェクト名 = new クラス名

Student stul = new Student();

**②変数・メソッド**
