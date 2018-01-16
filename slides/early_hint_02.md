### [Add preload_link_tag helper](https://github.com/rails/rails/pull/31251)

* rel="preload" によるコンテンツの先読みを行う為のメソッド

```ruby
preload_link_tag(post_path(format: :json), as: "fetch")
# => <link rel="preload" href="/posts.json" as="fetch" type="application/json" />
```

* ここでもEarly Hintsが使われている(リクエストがあればEarly Hintsを送信するようになっている)
