#### [Allow to pass a connection to the `dbconsole` command](https://github.com/rails/rails/commit/1acd9a6464668d4d54ab30d016829f60b70dbbeb)

* rails dbconsoleにconnection名を指定出来るようになった
  * bin/rails dbconsole -c replica
* 3-level database configurationを使っている場合に便利
  * なのだが、3-level database configuration自体がまだふんわりしている
