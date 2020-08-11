# テーブルを縦につなげる（UNION ALL）
- test

## 1 テープルの中身

![1](images/unionall1.png)

## 2 tempデータベース内に２つテーブル

![2](images/unionall2.png)

## 3 縦につなげる
![3](images/unionall3.png)

```SQL
SELECT * FROM test_news1
UNION ALL
SELECT * FROM test_news2;
```

- カラムが一致しないといけない


## 4 ※おまけ 日付（dateカラム）で並び替える
![4](images/unionall4.png)

```SQL
SELECT * FROM test_news1
UNION ALL
SELECT * FROM test_news2
ORDER BY date DESC;
```
