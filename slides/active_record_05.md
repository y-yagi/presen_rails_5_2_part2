#### [Disallow raw SQL in dangerous AR methods](https://github.com/rails/rails/pull/27947)

* 5.2時点ではdeprecateメッセージが表示されるだ、6.0ではUnknownAttributeReferenceがraiseされるようになる
* 引続き生SQLを渡すようにしたい場合、ActiveRecord::Base.allow_unsafe_raw_sqlに:disabledを指定すればOK
