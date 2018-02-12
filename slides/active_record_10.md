#### [Log the original call site for an ActiveRecord query](https://github.com/rails/rails/pull/26815)

* Active Recordのqueryが発行された際のcallersをログに表示するするようになった

```
# log/development.log
User Load (0.2ms)  SELECT "users".* FROM "users"
↳ app/views/users/index.html.erb:14
```

* 要は[active-record-query-trace](https://github.com/ruckus/active-record-query-trace)
* 表示されるのはserverのログでだけ(rails consoleでは出ない)
