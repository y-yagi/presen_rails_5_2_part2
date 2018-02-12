#### [Make `sanitize_sql_` methods public](https://github.com/rails/rails/commit/9d43a84f73c1b3853a91d052a462ee60eccaf957)

* sanitize_sql_xxxメソッド(sanitize_sql_likeとか、sanitize_sql_array等々)の可視性をpublicに変更した
* これにより、Modelの外から使用する際にsendを使う必要が無くなった
