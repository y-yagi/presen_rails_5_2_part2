### [credentials](https://github.com/rails/rails/pull/30067)

* Encrypted Secretsと異なり、基本的に必ずロードされる
  * `read_encrypted_secrets`相当のconfigは無い
* `require_master_key`はmaster key(データ復号の為のkey)が無い時の挙動を指定するためのもので、`read_encrypted_secrets`とは役割が違う
