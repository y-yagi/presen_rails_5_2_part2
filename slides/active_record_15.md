#### [Refactor Active Record to let Arel manage bind params](https://github.com/rails/rails/commit/213796fb4936dce1da2f0c097a054e1af5c25c2c)

* Active Recordで行っていたbind paramsの管理をArelで行うようリファクタリング
* ユーザに直接影響がある事はそんなに無い筈(private APIを使ってなければ)だが、bind parameterいじって何かしてたりしたらきをつけて
