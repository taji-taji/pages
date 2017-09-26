---
title: MySQLのTIMESTAMP型の日付の範囲
date: 2017-09-26 20:20:00 +0900
category: MySQL
---

# MySQLのTIMESTAMP型の日付の範囲

MySQLのTIMESTAMP型の日付のデータ範囲は下記の通り

- 下限：1970-01-01 00:00:01 +0000
- 上限：2038-01-19 03:14:07 +0000

それ以外は扱えないようなので、DATETIME型などを使用する。  
  
これはハマりそう、、

# 参考

https://qiita.com/ykawakami/items/2449a24e3b82ff0cbab6  
