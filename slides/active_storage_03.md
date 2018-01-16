### [ActiveStorage::Analyzer](http://edgeapi.rubyonrails.org/classes/ActiveStorage/Analyzer.html)

* blobからメタデータを取得する為の機能

```ruby
ActiveStorage::Analyzer::ImageAnalyzer.new(blob).metadata
# => { width: 4104, height: 2736 }
```

* デフォルトでは`ImageAnalyzer`と`VideoAnalyzer`が提供されている
