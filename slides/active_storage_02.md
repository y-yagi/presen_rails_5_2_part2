### Active Storage(前回からのアップデート)

* `rails new`時にActive Storage用のmigrationファイルを生成しなくなった
  * Active Storageを使いたい場合、明示的に`active_storage:install`を実行したmigrationファイルを生成する必要がある
  * 使いたいクラウドサービス用のgemを自分でGemfileに指定するのは変わらず必要(`aws-sdk-s3`、`google-cloud-storage`等)
* blobからメタデータを取得する為の機能が入った(ActiveStorage::Analyzer)
* blobのPreview機能が入った(ActiveStorage::Preview)
