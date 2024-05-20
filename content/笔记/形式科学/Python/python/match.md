##### match
- 在 Python 3.10 版本中引入了 `match` 语句，它是一种更强大、更可读的模式匹配语法。`match` 语句的目标是提供一种清晰、简洁地处理多个可能模式的方式，以替代传统的 `if-elif-else` 结构。
```python
def describe_value(value):
    match value:
        case 0:
            print("It's zero.")
        case 1 | 2:
            print("It's one or two.")
        case int if int > 2:
            print(f"It's greater than two: {value}")
        case str as s:
            print(f"It's a string: {s}")
        case _:
            print("It's something else.")

# 使用例子
describe_value(0)
describe_value(2)
describe_value(5)
describe_value("hello")
describe_value(True)

```