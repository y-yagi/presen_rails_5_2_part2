### [encrypted](https://github.com/rails/rails/commit/68479d09ba6bbd583055672eb70518c1586ae534)

```
$ EDITOR=vim bin/rails encrypted:edit config/staging-credentials.yml.enc
$ EDITOR=vim bin/rails encrypted:show config/staging-credentials.yml.enc
aws:
 access_key_id: 123
 secret_access_key: 345
```

```ruby
Rails.application.encrypted("config/staging-credentials.yml.enc")
# => #<ActiveSupport::EncryptedConfiguration:0x00562f5cfb8fd8 @key_path=#<Pathname:/home/yaginuma/program/rails/master/config/master.key>, @content_path=#<Pathname:/home/yaginuma/program/rails/master/config/staging-credentials.yml.enc>, @env_key="RAILS_MASTER_KEY">
```
