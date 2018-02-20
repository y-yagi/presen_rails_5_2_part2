#### [Add a #up_only method to migrations](https://github.com/rails/rails/pull/31082)

* migrationに`up`のときだけ使用出来る`up_only`メソッドが追加された

```ruby
class AddPublishedToPosts < ActiveRecord::Migration[5.2]
  def change
    add_column :posts, :published, :boolean, default: false
    up_only do
      execute "update posts set published = 'true'"
    end
  end
end
```
