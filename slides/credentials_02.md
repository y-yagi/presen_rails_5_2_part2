### [credentials](https://github.com/rails/rails/pull/30067)

* 基本的にはRails 5.1に入ったEncrypted Secretsと同じような感じ
  * リポジトリには暗号されたファイルが含まれ、そのファイルを編集・閲覧する為のコマンドが提供されている
* Encrypted Secretsと異なり、ファイルの構成はフラット
  * 環境毎に値を読めるようになっていない
