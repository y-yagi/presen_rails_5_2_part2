#### [Support Descending Indexes for MySQL](https://github.com/rails/rails/commit/606830d27a32fab23c0964b4383807fcdfdd7eba)

* Descending Indexが指定出来るようになった(MySQL 8.0.1以降)
  * e.g. "add_index [:firm_id, :type, :rating], name: "company_index", length: { type: 10 }, order: { rating: :desc }"
* 参考：[MySQL 8\.0 Labs – Descending Indexes in MySQL](http://mysqlserverteam.com/mysql-8-0-labs-descending-indexes-in-mysql/)
