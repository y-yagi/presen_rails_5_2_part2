### [credentials](https://github.com/rails/rails/pull/30067)

* `secret_key_base`も一つしか定義出来ないが、testやdevelopmentではどうするのか?
* -> test / development環境では自動でsecret_key_baseが生成されるようになり、[指定不要](https://github.com/rails/rails/blob/c2ba530c43244b5b60fd629f61cd8b44c43ecda9/railties/lib/rails/application.rb#L427..L435)
* staging :thinking_face:
