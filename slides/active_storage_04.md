### [ActiveStorage::Analyzer](http://edgeapi.rubyonrails.org/classes/ActiveStorage/Analyzer.html)

* `ImageAnalyzer`は`mini_magick`に、`VideoAnalyzer`は[ffmpeg](https://ffmpeg.org/)にそれぞれ依存している
  * ffmpegについては[直接コマンド叩いている](https://github.com/rails/rails/blob/c2ba530c43244b5b60fd629f61cd8b44c43ecda9/activestorage/lib/active_storage/analyzer/video_analyzer.rb#L84)
* 上記Analyzerを使用したい場合は、独自にAnalyzerを追加すればOK
