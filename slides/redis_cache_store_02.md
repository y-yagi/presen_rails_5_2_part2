### [Redis Cache Store](https://github.com/rails/rails/commit/9f8ec3535247ac41a9c92e84ddc7a3b771bc318b)

```ruby
config.cache_store = :redis_cache_store, driver: :hiredis,
  namespace: 'myapp-cache', compress: true, timeout: 1,
  url: "redis://:#{cache_password}@myapp-cache-1:6379/0"
```

* Rails guideの`Caching with Rails: An Overview`にRedis Storeについての説明が追加されているので、詳細はそちらを参照。[Caching with Rails: An Overview](http://edgeguides.rubyonrails.org/caching_with_rails.html#activesupport-cache-rediscachestore)

