#### [Recyclable cache keys](https://github.com/rails/rails/pull/29092)

* これにより、 ActiveRecord::Base#cache_versionの戻り値が変わっている(ActiveRecord::Base.cache_versioningがtrueの場合)

```ruby
# before
User.first.cache_key
# => "users/1-20180128010605891854"

# after
User.first.cache_key
# => "users/1"
```
