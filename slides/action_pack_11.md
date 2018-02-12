#### [Add Key Rotation to MessageEncryptor and MessageVerifier and simplify the Cookies middleware](https://github.com/rails/rails/pull/29716)

* これを利用してEncrypted Cookies及びSigned Cookiesのkeyのrotationが出来るようになった

```ruby
# signed cookies を SHA1 から SHA256に変更する場合
Rails.application.config.action_dispatch.signed_cookie_digest = "SHA256"

Rails.application.config.action_dispatch.cookies_rotations.tap do |cookies|
  cookies.rotate :signed, digest: "SHA1"
end
```
