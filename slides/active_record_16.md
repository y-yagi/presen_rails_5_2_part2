#### New error class

* LockWaitTimeout(最初はTransactionTimeoutだったが、後から LockWaitTimeoutにリネーム
  * [Add TransactionTimeout for MySQL error code 1205](https://github.com/rails/rails/pull/30360)
  * [Raise `TransactionTimeout` when lock wait timeout exceeded for PG ada…](https://github.com/rails/rails/commit/4a65dfcb9adae8fb12a86521c1a34b392e6084c2)
  * [Rename `TransactionTimeout` to more descriptive `LockWaitTimeout`](https://github.com/rails/rails/pull/31223)
