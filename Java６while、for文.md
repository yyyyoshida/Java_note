# while文

ある条件を満たす間ずっと処理を繰り返す

### for文なしのwhile文
```php
public class Loop1 {
    public static void main(String[] args) {
        int i = 0;
        while(i < 3) {
            System.out.println("i = " + i);
            i++;
        }
    }
}

>> i = 0
   i = 1
   i = 2
```

# for文

### シンプルなfor文
```php
public class Loop2 {
    public static void main(String[] args) {
        for(int i = 0; i < 3; i++) {
            System.out.println("i = " + i);
        }
    }
}

>> i = 0
   i = 1
   i = 2
```
### 配列を使ったfor文
```php
public class Loop3 {
    public static void main(String[] args) {
        int[] score = new int[5];
        score[0] = 80;
        score[1] = 100;
        score[2] = 75;
        score[3] = 0;
        score[4] = 30;

        String[] name = {"菅原", "村山", "寺山", "のび太", "ゴリラ"};

        for(int i = 0; i < score.length; i++) {
            System.out.println(name[i] + "さん" + score[i] + "点");
        }
        System.out.println("受験者数：" + score.length + "名");
    }    
}

>> 菅原さん80点
   村山さん100点
   寺山さん75点
   のび太さん0点
   ゴリラさん30点
   受験者数：4名
```
for文と配列は相性がいい
