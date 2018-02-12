#### [Allow passing a Proc or Symbol as an argument to length validator values](https://github.com/rails/rails/pull/30674)

* length validatorにProc, Symbolが渡せるようになった

```ruby
class Topic
  include ActiveModel::Validations

  attr_accessor :title, :foo

  validates :title, length: { maximum: ->(topic) { topic.max_length_for_title } }

  def max_length_for_title
    if foo
      5
    else
      10
  end
end
```
