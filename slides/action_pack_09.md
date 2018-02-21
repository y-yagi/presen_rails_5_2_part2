#### [Add expiry metadata to Cookies and freshen expires option to support duration](https://github.com/rails/rails/pull/30121)

* signed/encrypted cookiesに有効期限が指定出来るようになった


```ruby
# Sets a cookie that expires in 1 hour.
cookies[:login] = { value: "XJ-122", expires: 1.hour }

# Sets a cookie that expires at a specific time.
cookies[:login] = { value: "XJ-122", expires: Time.utc(2020, 10, 15, 5) }
```

* 有効期限後は値が読み込めなくなる
