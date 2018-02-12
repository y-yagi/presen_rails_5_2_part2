#### [AEAD encrypted cookies and sessions](https://github.com/rails/rails/pull/28132)

* encrypted cookiesにAES-256-GCMが使われるようになった
* なんでAEADが良いかは[コメント](https://github.com/rails/rails/pull/28132#issuecomment-282099566)参照
* 既存のcookiesについてはRails側で自動で新しいscheme使うようよしなにやってくれるので、特に対応は不要(Rails側にバグがなければ)
