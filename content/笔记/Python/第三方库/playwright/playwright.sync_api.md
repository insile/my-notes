##### playwright.sync_api
```python
from playwright.sync_api import sync_playwright, Playwright
```
- [[sync_playwright()]]  顶层API
---
- [[class Playwright]]  任务启动器
	- [[class BrowserType]]  特定浏览器启动器
		- [[class Browser]]  浏览器
			- [[class BrowserContext]] 浏览器上下文
			- [[class Page]] 页面
				- [[class Mouse]]  鼠标
				- [[class Keyboard]]  键盘
				- [[class Locator]]  定位器
	- [[class APIRequest]]  API测试启动器
		- [[class APIRequestContext]] 请求上下文
		- [[class APIResponse]] 响应

