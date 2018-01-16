### [Default Content Security Policy](https://github.com/rails/rails/pull/31162)

* デフォルトでちゃんとしているので、何も考えずにそのまま適用すると結構トラブルと思う
* [Upgrade CSP script_src default from unsafe_inline to nonce approach](https://github.com/rails/rails/issues/31689)
* config.content_security_policy_report_onlyにtrueを指定するとレポートだけを行う(ブロックはしない)モードになるので、ちょっと不安がある場合はそちらでとりあえず試してみるのが良いのでは無いでしょうか
