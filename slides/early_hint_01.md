### [HTTP/2 Early hints support](https://github.com/rails/rails/pull/30744)

* HTTP/2のEarly Hintsのサポートを`javascript_include_tag`、`stylesheet_link_tag`メソッドに追加
* デフォルトだとオフになっていて、サーバ起動時に`--early-hints`オプションを指定する必要がある
* Puma(3.11.0 以降)じゃないと今のところ動かない
  * Early Hints用のrack header(`rack.early_hints`)の対応が入っているのがPumaだけな為
