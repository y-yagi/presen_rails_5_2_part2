#### [Recyclable cache keys](https://github.com/rails/rails/pull/29092)

* fragments cachingのcache keyのフォーマットを再利用可能なフォーマットに変更
* 元々、デフォルトではcache keyにassocationのversion(timestamp)も含むようになっていた(e.g. projects/1-20170202145500)
  * デフォルトだとassociationのversionはupdated_atな為、レコードが更新される度に新しいkeyが生成されていた
  * 当然、その度に新しいcacheが生成される。結果、cacheがばかすか増える。
