#### [Drop the before_fork/on_worker_boot advice](https://github.com/rails/rails/commit/84cad15)

* 先の二つの対応により、Active Recordのconnectionを保持してるプロセスをforkした際のケアが不要になった

config/puma.rbに記載されていた

```ruby
before_fork do
  ActiveRecord::Base.connection_pool.disconnect! if defined?(ActiveRecord)
end
```

はもう不要


