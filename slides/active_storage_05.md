### [ActiveStorage::Preview](http://edgeapi.rubyonrails.org/classes/ActiveStorage/Preview.html)

* blobからPreview用の画像を作成する為の機能

```ruby
<%= image_tag file.preview(resize: "100x100>") %>
```

* デフォルトでは`PDFPreviewer`と`VideoPreviewer`が提供されている
