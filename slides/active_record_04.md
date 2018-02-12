#### [Disallow raw SQL in dangerous AR methods](https://github.com/rails/rails/pull/27947)

* orderとpluckの引数に生SQLをそのまま渡すのがdeprecateになった

```ruby
User.order("LENGTH(name)")
# => DEPRECATION WARNING: Dangerous query method (method whose arguments are used as raw SQL) called with non-attribute argument(s): "LENGTH(name)". Non-attribute arguments will be disallowed in Rails 6.0. This method should not be called with user-provided values, such as request parameters or model attributes. Known-safe values can be passed by wrapping them in Arel.sql().
```

* メッセージの通り、Arel.sqlメソッドでラップしてあげる必要がある
* Article.order(params[:my_order])のような形でメソッドを使用した場合に、SQL injectionが起こるのを防ぐ為、との事
