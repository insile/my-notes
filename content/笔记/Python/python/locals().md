- `locals( )`
	- 用于返回[[作用域和命名空间|当前作用域]]的局部变量和值的字典
	- 函数返回的字典是对实际变量的引用，因此实时更新，对字典的修改会影响变量本身
	- 在[[作用域和命名空间|当前作用域]]与[[vars()]]相等
	- 在[[作用域和命名空间|全局作用域]]与[[globals()]]，[[vars()]]相等
```python
def example_function():
    x = 10
    y = 'Hello'
    print(locals())  # {'x': 10, 'y': 'Hello'}
    print(locals()==vars())  # True

example_function()  


vars() == locals() == globals()  # True
```