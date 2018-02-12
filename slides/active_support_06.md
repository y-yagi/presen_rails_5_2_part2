#### [Use SHA-1 for non-sensitive digests by default](https://github.com/rails/rails/pull/31651)

* digestsの生成にMD5を使っていたのを、SHA-1を使うようになった
  * ETag headerとか
* config.active_support.use_hash_digest_classにdigest classを指定する事で、SHA-1以外を使用する事も可能
  * [Initial support for running Rails on FIPS-certified systems](https://github.com/rails/rails/pull/31289)
