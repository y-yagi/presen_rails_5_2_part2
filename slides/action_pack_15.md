#### [Add secure `X-Download-Options` and `X-Permitted-Cross-Domain-Policie…](https://github.com/rails/rails/commit/5d7b70f4336d42eabfc403e9f6efceb88b3eff44)

default headers setの変更。後から[Add 'Referrer-Policy' header to default headers set](https://github.com/rails/rails/commit/428939be9f954d39b0c41bc53d85d0d106b9d1a1)も入ったので、最終的には下記のようになっている(X-Download-Options以降が追加されたheader)。

```ruby
config.action_dispatch.default_headers = {
  "X-Frame-Options" => "SAMEORIGIN",
  "X-XSS-Protection" => "1; mode=block",
  "X-Content-Type-Options" => "nosniff",
  "X-Download-Options" => "noopen",
  "X-Permitted-Cross-Domain-Policies" => "none",
  "Referrer-Policy" => "strict-origin-when-cross-origin"
}
```
