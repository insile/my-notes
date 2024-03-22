##### class APIRequestContext
- `APIRequestContext.说明`
	- 用于 Web API 测试, 每个浏览器上下文都与其关联的请求上下文，该实例与浏览器上下文共享 cookie 存储，并且可以通过 [[class BrowserContext|BrowserContext.request]] 或 [[class Page|Page.request]] 进行访问
	- 如果您希望 API 请求不会干扰浏览器 cookie，则应通过调用 [[class APIRequest|APIRequest.new_context()]] 创建新的 APIRequestContext。此类对象将具有自己的独立 cookie 存储
- `APIRequestContext.实例方法`
```python
APIRequestContext.delete()
APIRequestContext.dispose()
APIRequestContext.fetch()
APIRequestContext.get()
APIRequestContext.head()
APIRequestContext.patch()
APIRequestContext.post()
APIRequestContext.put()
	# HTTP请求，返回 APIResponse
APIRequestContext.storage_state()
	# 返回此请求上下文的存储状态，包含当前 Cookie 和传递给构造函数的本地存储快照。返回字典
```

