#### [Allow mailers to configure their delivery job](https://github.com/rails/rails/pull/29457)

* delivery jobが固定のクラス(ActionMailer::DeliveryJob)だったのが、mailer毎に指定出来るようになった

```ruby
class MyMailer < ApplicationMailer
  self.delivery_job = MyCustomDeliveryJob

  # ...
end
```
