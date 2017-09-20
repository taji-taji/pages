---
title: HLS (HTTP Live Streaming)について
date: 2017-09-21 08:57:00 +0900
category: Audio-Video
---

## HLSとは？

`HTTP Live Streaming` の略で、動画をストリーミング送信するためのプロトコル。  
  
Appleによって開発されたもの。  
  
## 動画のフォーマット

- MPEG2-TS (MPEG2 transport stream)

#### 映像コーデック

- H.246

#### 音声コーデック

- AAC

## HLS構成要素

- `.ts`ファイル
  - 10秒ごとに細切れに複数作成される
  - 上記が帯域別にも作成される
- `.m3u8`ファイル
  - 上記`.ts`ファイルの再生順やファイルの場所などメタデータを扱う
  - どの`.ts`ファイルを再生するかを管轄する

## 特徴

- adaptive bitrate streaming
  - プレイヤーがコンテンツの再生状態を監視し、最適なビットレートへの切り替えをスムーズに行う

## 参考

- [https://developer.apple.com/streaming/](https://developer.apple.com/streaming/)
- [https://qiita.com/STomohiko/items/eb223a9cb6325d7d42d9](https://qiita.com/STomohiko/items/eb223a9cb6325d7d42d9)
- [http://bizvalley.co.jp/blog/1023.html](http://bizvalley.co.jp/blog/1023.html)
- [https://zencoder.com/ja/hls-guide](https://zencoder.com/ja/hls-guide)
