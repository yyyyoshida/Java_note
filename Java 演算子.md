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
```php
public class OpeIncrement {
  public static void main(String[] args) {
    int x = 1;
    int y = x++;
    System.out.println("yは" + y);   // 結果：yは1
    int a = 1;
    int b = ++a;
    System.out.println("bは" + b);   // 結果：bは2
  }
}
```
