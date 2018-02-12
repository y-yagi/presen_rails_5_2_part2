#### [Change sqlite3 boolean serialization to use 1 and 0](https://github.com/rails/rails/pull/29699)

* SQLite 3 adapterでbooleanの値を保持するのにStringのt / fを使用していたのを、Integer(`1` / `0`)を使用するよう修正した
  * 1と0はSQLite側でも true / falseと認識する為(t / fではtrue / falseとは認識されない)。
* 元々`t` / `f`で保持していた値は、手動で移行する必要がある(e.g. ExampleModel.where("boolean_column = 't'").update_all(boolean_column: 1))
