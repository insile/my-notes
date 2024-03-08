##### 类的定义与实例化
- 类的定义
	- 使用 [[class]] 保留字
	- 在这个示例中，我们定义了一个名为 `Person` 的类，它具有两个属性 `name` 和 `age`，以及一个方法 `greet()`
```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def greet(self):
        print(f"Hello, my name is {self.name} and I am {self.age} years old.")
```
- 类的实例化
	- 实例化类是指创建类的对象，通常是将类看作一个函数去调用 `object = Classname(args)`
	- 实例化通过构造方法 [object.\_\_new\_\_()](object.__new__()) 和初始化方法 [object.\_\_init\_\_()](object.__init__()) 来创建一个实例
```python
# 创建一个 Person 对象
person1 = Person("Alice", 30)
person1.greet()  # 调用对象的方法

# 创建另一个 Person 对象
person2 = Person("Bob", 25)
person2.greet()

```