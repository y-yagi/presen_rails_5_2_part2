### [credentials](https://github.com/rails/rails/pull/30067)

* secrets.yml.enc

```yml
production:
  external_api_key: 1466aac22e6a869134be3d09b9e89232fc2c2289
```

* credentials.yml.enc

```yml
aws:
 access_key_id: 123
 secret_access_key: 345

# Used as the base secret for all MessageVerifiers in Rails, including the one protecting cookies.
secret_key_base: bfae0e7ae2106467b0b082188c9da6b6004d108aa20f6445555097e4e6207419d09dfc2bc0db670e7583528c0fe1ca06eb72aedd8f7d17653d431ef877e8fb5e
```
