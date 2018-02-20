#### [Add bootsnap to default Gemfile](https://github.com/rails/rails/pull/29313)

* デフォルトで生成されるGemfileにbootsnapが追加された
* Gemfileにbootsnapを追加、及び、config/boot.rbでbootsnap/setupをrequireするようになっただけ
* rails newに--skip-bootsnapオプションも追加済み
