#### [Add Key Rotation to MessageEncryptor and MessageVerifier and simplify the Cookies middleware](https://github.com/rails/rails/pull/29716)

* MessageEncryptor`クラス及びMessageVerifierクラスにkey rotationのサポートを追加
* それぞれrotateメソッドが提供されおり、keyのrotationが出来るようになっている

```ruby
old_secret  = SecureRandom.random_bytes(32)
old_message = ActiveSupport::MessageEncryptor.new(old_secret, cipher: "aes-256-gcm").encrypt_and_sign("old")

new_secret  = SecureRandom.random_bytes(32)
encryptor = ActiveSupport::MessageEncryptor.new(new_secret, cipher: "aes-256-gcm")
encryptor.rotate(old_secret)

encryptor.decrypt_and_verify(old_message) # => "old"
```

