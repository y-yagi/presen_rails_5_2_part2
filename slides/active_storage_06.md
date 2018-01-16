### [ActiveStorage::Preview](http://edgeapi.rubyonrails.org/classes/ActiveStorage/Preview.html)

* `PDFPreviewer`は[mupdf](https://mupdf.com/)に、`VideoPreviewer`は[ffmpeg](https://ffmpeg.org/)にそれぞれ依存している
  * どっちもコマンド直接叩いている
* PDFの場合は最初のページが、Videoの場合は最初のフレームがpreview画像として使用される
* 上記Analyzerを使用したい場合は、独自にAnalyzerを追加すればOK
