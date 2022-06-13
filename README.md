## 概要

SSL 証明書の検証用。

## 使い方

* conf ディレクトリに以下のファイルを置く。

```
server.crt    -- 証明書
server.key    -- 秘密鍵
server-ca.crt -- CA 中間証明書
```

* 起動する。

```
docker-compose up
```

* 自分の端末の hosts ファイルにある 127.0.0.1 に対し、その証明書のドメインを追加する。

```
sudo vi /etc/hosts
127.0.0.1 localhost example.com
```

* ブラウザでアクセスする。  
https://example.com/

