#### [Improve AR connection fork safety](https://github.com/rails/rails/pull/31173)

* Active Recordのconnectionを保持するプロセスをforkした際、親プロセスに属しているconnectionを破棄するようになった
  * 子プロセスで親プロセスのconnectionに対して誤ってquit/shutdown/goodbye等のメッセージ送信しないようにする為
