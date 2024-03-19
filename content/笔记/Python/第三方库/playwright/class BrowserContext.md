##### class BrowserContext
- `BrowserContext.说明`
	- 浏览器上下文提供了一种操作多个独立浏览器会话的方法。
	- 如果一个页面打开另一个页面, 弹出窗口将属于父页面的浏览器上下文。
	- 通过[[Browser.new_context()]]创建, 支持创建隐身浏览器上下文, 不会将任何浏览数据写入磁盘。
```python
context = browser.new_context()  # 浏览器上下文
page = context.new_page()  # 在上下文中创建一个新页面
page.goto("https://example.com")  # 导航前往
context.close()  # 关闭上下文
```
- `BrowserContext.实例方法`
```python
BrowserContext.add_cookies()
	# 将 Cookie 添加到此浏览器上下文中
BrowserContext.clear_cookies()
	# 清除上下文 Cookie。
BrowserContext.cookies()
	# 如果未指定 URL，则此方法返回所有 Cookie。如果指定了 URL，则仅返回影响这些 URL 的 Cookie。

BrowserContext.add_init_script()
	# 添加初始化脚本的方法
BrowserContext.clear_permissions()
	# 清除浏览器上下文的所有权限覆盖。
BrowserContext.close()
	# 关闭浏览器上下文。属于浏览器上下文的所有页面都将关闭。

BrowserContext.expect_console_message()
	# 执行操作并等待控制台消息在上下文中的页面中记录。如果提供了谓词，它将控制台消息值传递到函数中，并等待返回真实值。
BrowserContext.expect_event()
BrowserContext.expect_page()
BrowserContext.expose_binding()
BrowserContext.expose_function()
BrowserContext.grant_permissions()
BrowserContext.new_cdp_session()
BrowserContext.new_page()
BrowserContext.route()
BrowserContext.route_from_har()
BrowserContext.set_default_navigation_timeout()
BrowserContext.set_default_timeout()
BrowserContext.set_extra_http_headers()
BrowserContext.set_geolocation()
BrowserContext.set_offline()
BrowserContext.storage_state()
BrowserContext.unroute()
BrowserContext.wait_for_event()
```