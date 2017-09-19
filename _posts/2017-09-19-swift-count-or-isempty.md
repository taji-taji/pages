---
title: 【Swift】 Collectionが空かどうかはcountよりもisEmptyを使う
date: 2017-09-19 17:43:00 +0900
categories: Swift
---

# count == 0 vs isEmpty

表題の通り。Collectionが空かどうかは`isEmpty`を使った方が良い。  
対象のCollectionが`RandomAccessCollection`に準拠していない場合、Collectionの要素を反復的に処理する。
パフォーマンスとしてよくないので、習慣的に`count == 0`の空チェックは使わない方が良さそう。

# 参考

https://developer.apple.com/documentation/swift/array/1688398-isempty
https://developer.apple.com/documentation/swift/dictionary/2886696-isempty
https://qiita.com/a-beco/items/bf740ed9c8e4575e64b2
