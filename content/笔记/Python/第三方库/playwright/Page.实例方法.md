##### Page.实例方法
- Page.基础操作
```python
Page.goto()
	# 导航到指定的 URL。返回 Response 实例
Page.reload()
	# 此方法重新加载当前页，方式与用户触发浏览器刷新相同。返回 Response 实例
Page.go_back()
	# 在浏览器历史记录中后退一步。返回 Response 实例
Page.go_forward()
	# 在浏览器历史记录中前进一步。返回 Response 实例
Page.close()
	# 关闭页面
Page.content()
	# 获取页的完整 HTML 内容，包括 doctype。返回 str
Page.opener()
	# 用于获取打开当前页面的父页面。返回 Page.实例
Page.pause()
	# 暂停脚本执行
Page.pdf()
	# 打印pdf。返回 bytes
Page.screenshot()
	# 截图。返回 bytes
Page.title()
	# 返回页面的标题。
```
- Page.定位器
```python
Page.locator()
	# 返回一个元素定位器。返回 Locator 实例
Page.get_by_alt_text()
	# 根据元素的 alt 文本定位。返回 Locator 实例
Page.get_by_label()
	# 根据元素的标签定位。返回 Locator 实例
Page.get_by_placeholder()
	# 允许通过占位符文本定位输入元素。返回 Locator 实例
Page.get_by_role()
	# 允许根据 ARIA 角色、 ARIA 属性和可访问名称定位元素。返回 Locator 实例
Page.get_by_test_id()
	# 通过测试 ID 定位元素。返回 Locator 实例
Page.get_by_text()
	# 允许定位包含给定文本的元素。返回 Locator 实例
Page.get_by_title()
	# 允许根据标题属性定位元素。返回 Locator 实例
```
- Page.期望
```python
Page.expect_console_message
Page.expect_download
Page.expect_event
Page.expect_file_chooser
Page.expect_popup
Page.expect_request
Page.expect_request_finished
Page.expect_response
Page.expect_websocket
Page.expect_worker
```
- Page.导航操作
```python
Page.add_init_script
Page.add_script_tag
Page.add_style_tag
Page.bring_to_front
Page.drag_and_drop
Page.emulate_media
Page.evaluate
Page.evaluate_handle



Page.expose_binding
Page.expose_function

Page.frame
Page.frame_locator

Page.route
Page.unroute
Page.route_from_har
Page.set_content
Page.set_default_navigation_timeout
Page.set_default_timeout
Page.set_extra_http_headers
Page.set_viewport_size

Page.wait_for_event
Page.wait_for_function
Page.wait_for_load_state
Page.wait_for_url
```
