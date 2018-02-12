#### [Add option for class_attribute default](https://github.com/rails/rails/pull/29270)

* class_attributeにdefaultオプションが追加された
  * "class_attribute :_layout_conditions, instance_accessor: false, default: {}"みたいに書ける
* mattr_accessor、及び、関連メソッドにも同様にdefaultオプションが追加された
  * [Introduce mattr_accessor default option](https://github.com/rails/rails/pull/29294)
