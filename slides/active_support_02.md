#### [ActiveSupport::CurrentAttributes provides a thread-isolated attributes singleton](https://github.com/rails/rails/pull/29180)

* スレッド毎に独立したattibutesを管理するためのActiveSupport::CurrentAttributesクラスが追加された
  * リクエスト毎のattribute(リクエストIDやUA等)をシステム全体で使用可能にする、のが主なユースケースとの事
  * リクエトの前後で自動でattributeのresetが行われるようになっている
* 具体的な使い方は[Doc](http://edgeapi.rubyonrails.org/classes/ActiveSupport/CurrentAttributes.html)参照
