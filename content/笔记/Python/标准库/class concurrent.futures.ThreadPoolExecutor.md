##### class concurrent.futures.ThreadPoolExecutor
- `ThreadPoolExecutor.创建`
```python
ThreadPoolExecutor(max_workers=None, thread_name_prefix='', initializer=None, initargs=())
# max_workers 最大线程数
# thread_name_prefix 线程的名称前缀
```
##### 示例
```python
from concurrent.futures import ThreadPoolExecutor


def task(name: str):
    """
    定义一个任务函数，接受一个名称参数，并打印任务执行的步骤。
    :param name: str, 任务名称
    :return: str, 任务完成消息
    """
    print(f'{name} - step 1\n', end='')
    print(f'{name} - step 2\n', end='')
    return f'{name} complete'


# 创建一个 ThreadPoolExecutor 对象，并使用 submit() 方法提交任务
with ThreadPoolExecutor() as execute:
    r1 = execute.submit(task, 'A')  # 返回 Future 
    r2 = execute.submit(task, 'B')
	
    print(r1.result())
    print(r2.result())

# 创建另一个 ThreadPoolExecutor 对象，并使用 map() 方法提交任务
with ThreadPoolExecutor() as execute:
    r3 = execute.map(task, ['C', 'D'])  # 返回存储结果迭代器
	
    for r in r3:
        print(r)

```