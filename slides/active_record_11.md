#### [Add bulk alter support for PostgreSQL](https://github.com/rails/rails/pull/31331)

* PostgreSQL adapterにbulk alterのサポートを追加
* PostgreSQLでもchange_tableにbulk: trueオプションを指定した場合、一つのALTER TABLEでSQLが実行されるようになった
