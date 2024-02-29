##### bytearray类型
- 可变的二进制格式字节数据数组
- 字节数组（bytearray）是一种类似于列表的数据类型，它存储一系列的字节（bytes）值，并允许您对这些字节进行修改。
- [[序列方法]]
##### 创建字节数组
- [[bytearray()]]
```python
# 创建一个空的字节数组
empty_bytearray = bytearray()
print(empty_bytearray)  # 输出：bytearray(b'')

# 创建一个包含字节的字节数组
bytearray_with_data = bytearray(b'hello')
print(bytearray_with_data)  # 输出：bytearray(b'hello')

byte_array = bytearray(b'hello')
byte_array[0] = 72  # 修改第一个字节为 ASCII 值 72 (H)
byte_array[1:3] = b'XY'  # 修改索引 1 到 2 的字节为 XY
print(byte_array)  # 输出：bytearray(b'HXYlo')
```