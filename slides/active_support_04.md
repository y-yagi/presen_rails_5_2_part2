#### [Add next and previous day of week api to ActiveSupport](https://github.com/rails/rails/pull/26600)

* 次、又は、前の曜日を取得するためのDate#prev_occurring、Date#next_occurringメソッドが追加された

```ruby
Date.today
# => Wed, 31 May 2017
Date.today.next_occurring(:monday)
# => Mon, 05 Jun 2017 00:00:00 UTC +00:00
Date.today.prev_occurring(:monday)
# => Mon, 29 May 2017 00:00:00 UTC +00:00
```
