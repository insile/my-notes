##### for 语句
- 循环语句，按照一定次数循环执行一组语句
- [[for]]
- 可用于遍历[[迭代器类型|可迭代对象]]，按顺序逐个访问其中的元素，从而对每个元素执行相应的操作
- for 循环本质就是调用[[迭代器类型|可迭代对象]]的[[object.__iter__()]]方法获得一个迭代器，然后不断调用迭代器[[object.__next__()]]方法实现的
```python
'''
for 变量 in 可迭代对象
	循环体
'''

fruits = ["apple", "banana", "orange"]
for fruit in fruits:
    print(fruit)
```
- 结合函数[[range()]]，循环计数控制
```python
'''
for 变量 in range()
	循环体
'''

for i in range(5):
    print(i)

for _ in range(5):
    # 循环5次，但不用这个变量_
```
