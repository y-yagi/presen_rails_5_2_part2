#### [Flush idle database connections](https://github.com/rails/rails/pull/31221)

* idle状態のコネクションを自動で切断するようになった
* デフォルトでは300秒以上使われていないコネクションが自動で切断されるようになっている
  * 切断までの時間はconfig(idle_timeout)で変更可能
