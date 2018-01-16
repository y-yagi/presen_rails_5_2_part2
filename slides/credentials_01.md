### [credentials](https://github.com/rails/rails/pull/30067)

* 秘密情報を管理する為の仕組み
* 現状、秘密情報を保持する為のファイルが複数(`config/secrets.yml`、`config/secrets.yml.enc`)あり、かつ、それらのファイルとは別に`SECRET_BASE_KEY`という環境変数があったりで、ややこしい状態になていた
* また、"secrets"という名前があまり良くないのでは、という思いもあったらしく、別途"credentials"という仕組みが入った
