# genjws
## 概要
RSA-SHA256で署名されたJWTをシェルスクリプトで作成するサンプル。

- 動作確認には https://jwt.io/ を利用
- opensslコマンドが必要

## 使い方
1. 秘密鍵を入手してスクリプトと同じ場所に「private_key」という名前で保存する
2. スクリプト中の用意されたペイロードを実際に送信したいJSONデータへ書き換える
3. スクリプトを実行する
4. JWSが表示される

### 実行イメージ
```console
$ ls
genjwt  private_key

$ ./genjwt 
eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiYWRtaW4iOnRydWV9.EkN-DOsnsuRjRO6BxXemmJDm3HbxrbRzXglbN2S4sOkopdU4IsDxTI8jO19W_A4K8ZPJijNLis4EZsHeY559a4DFOd50_OqgHGuERTqYZyuhtF39yxJPAjUESwxk2J5k_4zM3O-vtd1Ghyo4IbqKKSy6J9mTniYJPenn5-HIirE
```
