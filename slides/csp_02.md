### [Default Content Security Policy](https://github.com/rails/rails/pull/31162)

```ruby
# config/initializers/content_security_policy.rb
Rails.application.config.content_security_policy do |policy|
  policy.default_src :self, :https
  policy.font_src    :self, :https, :data
  policy.img_src     :self, :https, :data
  policy.object_src  :none
  policy.script_src  :self, :https, :unsafe_inline
  policy.style_src   :self, :https, :unsafe_inline

  # Specify URI for violation reports
  # policy.report_uri "/csp-violation-report-endpoint"
end
```

```ruby
class PostsController < ApplicationController
  content_security_policy do |p|
    p.upgrade_insecure_requests true
    p.base_uri :self, -> { "https://#{current_user.domain}.example.com" }
  end
end
```
