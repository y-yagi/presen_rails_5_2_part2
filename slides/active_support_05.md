#### [Cache: write_multi](https://github.com/rails/rails/pull/29366)

* ActiveSupport::Cache::Storeに`write_multi`メソッドが追加された
  * 名前の通りで複数データをまとめて書き込む為のメソッド
  * e.g. Rails.cache.write_multi foo: 'bar', baz: 'qux'
* Redis adapterだとMSETを使うようになるので、一個一個書き込むよりはやい
* 他のadapterは、(今の所)複数回write_entryするだけなの性能的には変わらない
