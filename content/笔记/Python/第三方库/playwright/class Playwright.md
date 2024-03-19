##### class Playwright
- `Playwright.说明`
	- 这是剧作家, 启动任务的开始, 通过[[sync_playwright()]]创建
```python
from playwright.sync_api import sync_playwright

def run(playwright):  # 运行一个Playwright实例
    chromium = playwright.chromium  # 返回 BrowserType 的实例
    browser = chromium.launch()  # 启动
    page = browser.new_page()
    page.goto("http://example.com")
    # other actions...
    browser.close()

with sync_playwright() as playwright:
    run(playwright)  # 通过上下文管理器创建了Playwright实例
```
- `Playwright.实例方法`
```python
playwright.stop()
	# 终止此 Playwright 实例
	# 上下文管理器结束时自动终止
```
- `Playwright.实例属性`
```python
playwright.chromium
	# 此对象可用于启动或连接 Chromium，返回 BrowserType 的实例。
playwright.firefox
	# 此对象可用于启动或连接到 Firefox，返回 BrowserType 的实例。
playwright.webkit
	# 此对象可用于启动或连接到 WebKit，返回 BrowserType 的实例。

playwright.request
	# 公开可用于 Web API 测试的 API，返回 APIRequest 的实例。

playwright.selectors
	# 选择器，返回 Selectors 的实例。

playwright.devices
	# 返回与 Browser.new _ context ()或 Browser.new _ page ()一起使用的设备字典。
```