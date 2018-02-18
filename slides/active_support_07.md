#### [Add support for connection pooling on RedisCacheStore](https://github.com/rails/rails/pull/31866)

* redis cache storeにconnection poolingのサポートを追加
* ool_sizeオプションを指定した場合のみconnection poolが使用されるようになってる
* connection pool部分の実装は[mperham/connection\_pool](https://github.com/mperham/connection_pool) gemを使用している
* mem cache storeでも同様のサポートが入っている
  * [Support for connection pooling on mem cache store](https://github.com/rails/rails/commit/4ac143d1937e8d6f33162863a17c1b1db57687c1)
