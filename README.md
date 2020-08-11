# テーブルを縦につなげる（UNION ALL）
- test

## 1

![1](images/unionall1.png)

## 2

![2](images/unionall2.png)

## 3
![3](images/unionall3.png)

```SQL
SELECT * FROM test_news1
UNION ALL
SELECT * FROM test_news2;
```

## 4 aaa
![4](images/unionall4.png)

```SQL
SELECT * FROM test_news1
UNION ALL
SELECT * FROM test_news2
ORDER BY date DESC;
```
