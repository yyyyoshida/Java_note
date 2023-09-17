
# else - if文

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

//---------------------------------------------------------------------------------------------------------------------------

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

> java Branch1 4500

>> 値引金額：300円
   税金金額：4620円

> java Branch1 6700

>> 値引金額：500円
   税金金額：6820円

```

# switch文

### 記述できる値の制限

switch-case文で使える型は決まっていて、int、short、char、byte、enum、Stringの6つだけ

### 入力する数値に該当する人の入園料が出てくるコード

```php
public class Branch2 {
    public static void main(String[] args) {
        int num = Integer.parseInt(args[0]);
        switch(num) {
            case 1:
              System.out.println("入園料金:8400円");
              break;
            case 2:
              System.out.println("入園料金:7000円");
              break;
            case 3:
              System.out.println("入園料金:5000円");
              break;
            default:
              System.out.println("1:一般, 2:中・高校生, 3:小学生・幼児");
        }
    }  
}

> java Branch2 0

>> 1:一般, 2:中・高校生, 3:小学生・幼児


> java Branch2 1

>> 入園料金:8400円


> java Branch2 2

>> 入園料金:7000円


> java Branch2 3

>> 入園料金:5000円
```


### 入力する曜日に該当する曜日が出てくるコード

```php
public class SwitchSample {
    public static void main(String[] args) {
        String week = "Friday";
     
        switch (week) {
        case "Sunday":
            System.out.println("日曜日");
            break;
        case "Monday":
            System.out.println("月曜日");
            break;
        case "Tuesday":
            System.out.println("火曜日");
            break;
        case "Wednesday":
            System.out.println("水曜日");
            break;
        case "Thursday":
            System.out.println("木曜日");
            break;
        case "Friday":
            System.out.println("金曜日");
            break;
        case "Saturday":
            System.out.println("土曜日");
            break;
        default:
            System.out.println("不明な曜日");
        }
    }
}

>> 金曜日
```







