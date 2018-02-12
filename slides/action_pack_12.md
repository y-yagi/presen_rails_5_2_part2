#### [Add headless chrome driver to System Tests](https://github.com/rails/rails/pull/30876)

* System testにheadless chrome driverのサポートが追加された

```ruby
class DrivenBySeleniumWithHeadlessChrome < ActionDispatch::SystemTestCase
  driven_by :selenium, using: :headless_chrome
end
```

* headless firefox driverのサポートも追加された
  * [Add headless firefox driver to System Tests](https://github.com/rails/rails/commit/82b974813b28748e5affcff1d8c4ad60ab2971be)
