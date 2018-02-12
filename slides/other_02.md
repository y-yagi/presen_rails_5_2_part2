#### Use frozen string literal

* Railsのコードすべてに対してfrozen string literalが指定されるようになりました
  * [Use frozen-string-literal in ActiveSupport](https://github.com/rails/rails/commit/72950568dde05bfe8a69ce4bbf6338fdebf3062f)
  * [Use frozen string literal in actionmailer/](https://github.com/rails/rails/commit/82df8c2ca545785cd49f8c9552a054a05e6ac289)
  * 以下略
* Railsのバージョンをあげたらいきなり"can't modify frozen String"が出るようになった場合、Rails側の問題の可能性もあるので、issueください
  * JRubyとかあやしい
