# iOSのアプリを開発して申請するまでに味わった苦しみ

## 目次

- はじめに
- 証明書
   - 証明書の種類
   - 証明書の関連性
   - 署名書の作り方
- AppStore Connectについて
   - アプリの作り方
   - バージョンの作り方

## 1. はじめに

iOSアプリを開発し終わり、さて申請するぞ、となった皆さん、おめでとうございます！
開発工程までは本やら記事やらで様々な情報を手に入れることができたと思いますが、いざ申請してAppStoreの大海原へ繰り出すぞ！ となるタイミングで途端に情報が少なくなるような気がしています。実際に僕が申請をしてみるときにも、わからないことが噴出してなんどもなんどもQiitaとにらめっこしました。
というわけで、経験した範囲で今回体験したリリース用ビルドから申請まで記録をしておきたいと思います。

## 2. 証明書

iOSアプリ申請でのめんどくさいやつNo.1(主観が含まれております)、証明書。
Apple Developerで証明書を扱ったことがある人ならわかってもらえると思いますが、Apple Developerの証明書というのはとにかくわかりづらいです。
.csr、.cer、.p12……と色々と種類があり、しかもそれらが互いに紐づいているため、組み合わせを取り違えてしまうと、種類は合っているのにどうにもエラーが出て先に進めないと言ったことにもなりがちです。

### 2-1. 証明書の種類
