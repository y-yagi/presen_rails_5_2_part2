#### [Eager load controller actions to reduce response time of the first request](https://github.com/rails/rails/pull/29559)

* eager_load = trueの場合に、各controllerのactionメソッドをサーバ起動時に読む込むよう変更
* 元々は最初のリクエスト実行時に読みこむようになっていたが、それだと最初のリクエストのreponse timeが遅くなってしまう為、それを避ける為、サーバ起動時に読みこむようになりました
