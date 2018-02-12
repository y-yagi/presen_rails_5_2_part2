#### [Do not generate default alt text for images](https://github.com/rails/rails/pull/30213)

* 上記の場合、スクリーンリーダーは、"Logo"というテキストを読みあげる
* が、これは実際は何も意味もない情報(logo.pngが会社のロゴならその会社名が読み上げらないと意味が無い)
* というわけで、デフォルトで生成されるalt属性には意味がない、どころが邪魔になってしまっている、という事でデフォルトではalt属性を生成しないようにしたとの事
