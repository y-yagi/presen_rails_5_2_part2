#### [Build a multi-statement query when inserting fixtures](https://github.com/rails/rails/pull/31422)

* fixturesをinsertする際に、multi statement queryを使用するようになった
* これにより、元々はtable毎にqueryを実行していたのを、一つのqueryでまとめてデータを作成(削除も)するようになった
