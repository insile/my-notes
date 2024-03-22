##### class Browser
- `Browser.说明`
	- 具体的浏览器对象, 通过[[BrowserType.launch()]]创建
```python
from playwright.sync_api import sync_playwright

def run(playwright):
    firefox = playwright.firefox
    browser = firefox.launch()  # 浏览器实例, 默认无头
	# browser = firefox.launch(headless= False)  # 有头
    page = browser.new_page()
    page.goto("https://example.com")
    browser.close()

with sync_playwright() as playwright:
    run(playwright)
```
- `Browser.实例方法`
	- [[Browser.new_context()]]  创建浏览器上下文
	- [[Browser.new_page()]]  便捷新单页
```python
Browser.close()
	# 如果浏览器是创建的，关闭浏览器及其所有页面
	# 如果浏览器是连接的，清除属于此浏览器的所有已创建上下文，并断开与浏览器服务器的连接
```
