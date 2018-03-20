---
title: 【MySQL】MySQLの特定のカラムのcharsetとcollateを変える
date: 2018-03-20 10:22:00 +0900
categories: MySQL
---

# MySQLの特定のカラムのcharsetとcollateを変える

## 絵文字対応したい

```sql
alter table `table_name` modify `target_column_name` text character set utf8mb4 collate utf8mb4_bin not null;
```

その他、MySQLサーバーの設定やクライアント側の設定も変更の必要あり。
下記、参考：

- [[MySQL] iPhoneやAndroidの絵文字を格納するにはutf8mb4を文字コードにしないといけない](https://www.scriptlife.jp/contents/programming/2016/03/21/post-1454/)
- [mysqlでiPhone絵文字対応したときのメモ](http://kimagureneet.hatenablog.com/entry/2015/01/17/110000)
- [Rails 5 と MySQL 5.6 環境における utf8mb4 を扱う設定について](https://qiita.com/dany1468/items/6431e486b8949cadcbe0)
- [MySQLの文字コード事情 2017版](https://qiita.com/dany1468/items/6431e486b8949cadcbe0)
