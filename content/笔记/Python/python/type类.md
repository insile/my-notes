##### type类
- type类 是内置[[元类的定义与实例化|元类]]，用于创建其他类
- type类 继承自 [[object类]]，object类 是 type类 的父类
- [[type()]] 创建type类实例，就是一个类对象
```python
print(type)  # <class 'type'> type 类

type(object())  # object实例的类型 <class 'object'>
type(object)  # object类的类型 <class 'type'>
type(type)  # type类的类型 <class 'type'>
type.__bases__  # type 继承的父类 (<class 'object'>,)
```