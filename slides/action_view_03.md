#### [Do not generate default alt text for images](https://github.com/rails/rails/pull/30213)

* imageタグを生成する際、デフォルトではalt属性を生成しないようになった
* 元々は、image_tag "logo.png"だと、下記のようなHTMLが生成されていた

```html
<img src="/images/logo.png" alt="Logo" />
```
