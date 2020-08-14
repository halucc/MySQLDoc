# テーブルを縦につなげる（UNION ALL）

LIKE演算子を用いて、複数のテーブルから検索する場合などに使用する


## 1 【準備】tempデータベース

```SQL
SHOW TABLES;
```

![2](images/unionall2.png)

## 2 テーブルの中身

![1](images/unionall1.png)


## 3 縦につなげる
![3](images/unionall3.png)

```SQL
SELECT * FROM test_news1
UNION ALL
SELECT * FROM test_news2;
```

※カラム（id,title,date）は一致していなければならない


## 4 日付（dateカラム）で並び替える
![4](images/unionall4.png)

```SQL
SELECT * FROM test_news1
UNION ALL
SELECT * FROM test_news2
ORDER BY date DESC; -- ORDER BY // ソート
-- DESC // 降順
-- ASC // 昇順
```
