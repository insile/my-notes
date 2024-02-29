- 在一个协程函数中运行其他协程函数, 等待异步操作完成
- 挂起该协程函数的执行以等待一个 [[可等待对象]]。 只能在 [[协程]] 内部使用。
- [[asyncio 库]]
```python
import asyncio
import time

async def say_after(delay, what): # 子协程
    await asyncio.sleep(delay)
    print(what)

async def main(): # 主协程
    print(f"started at {time.strftime('%X')}")

	# 主协程挂起，等待子协程
    await say_after(1, 'hello') # 等待子协程 1 s
    await say_after(2, 'world') # 等待子协程 2 s

    print(f"finished at {time.strftime('%X')}")  # 共等 3 s

asyncio.run(main())
# 事件循环处理主协程
```