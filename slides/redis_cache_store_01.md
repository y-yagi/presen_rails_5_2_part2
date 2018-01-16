### [Redis Cache Store](https://github.com/rails/rails/commit/9f8ec3535247ac41a9c92e84ddc7a3b771bc318b)

* Railsがデフォルトでサポートするcache storeに、Redis cache storeが追加された
* 他のcache store同様に、:namespace、:compress、:compress_threshold, :expires_in, :race_condition_tool等のオプションが指定出来るようになっている
* driverが指定出来るようになっており、redis-rbだけでなく、hiredis, Redis::Distributedが指定出来るようになっている

