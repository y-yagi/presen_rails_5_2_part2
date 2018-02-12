#### attributes API?

* Active Recordにあったattributes API用のclass / moduleがActive Model配下に移動された
  * [Start bringing attributes API to AM](https://github.com/rails/rails/pull/30920)
  * [Move Attribute and AttributeSet to ActiveModel](https://github.com/rails/rails/pull/30985)
* これにより、Active Modeldでもattributes APIが使えるようにはなっている
* ただ、まだpublic APIではないからね
  * https://github.com/rails/rails/pull/31848#issuecomment-362130685
