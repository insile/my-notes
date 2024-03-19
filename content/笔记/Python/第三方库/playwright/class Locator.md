##### class Locator
- `Locator.说明`
	- 定位器代表了一种随时在页面上查找元素的方法
	- 每个页面对象可以通过 [[Page.实例方法|Page.定位器]] 创建
```python
page.get_by_label("User Name").fill("John")

page.get_by_label("Password").fill("secret-password")

page.get_by_role("button", name="Sign in").click()

expect(page.get_by_text("Welcome, John!")).to_be_visible()
```
- `Locator.实例方法`
```python
Locator.evaluate
	# 在页面中执行 JavaScript 代码，将匹配元素作为参数
Locator.evaluate_all
	# 在页面中执行 JavaScript 代码，将所有匹配的元素作为参数
Locator.evaluate_handle
	# 在页面中执行 JavaScript 代码，将匹配元素作为参数，并返回带有结果的 JSHandle
Locator.fill
	# 输入值
Locator.filter
	# 继续过滤，缩小现有定位器的范围
Locator.focus
	# 将焦点设置在指定的元素上
Locator.frame_locator
	# 在使用 iframe 时，您可以创建一个框架定位器，该定位器将输入 iframe 并允许定位该 iframe 中的元素
Locator.get_attribute
	# 返回匹配元素的属性值
Locator.get_by_alt_text
	# 允许按替换文本查找元素
Locator.get_by_label
Locator.get_by_placeholder
Locator.get_by_role
Locator.get_by_test_id
Locator.get_by_text
Locator.get_by_title
Locator.highlight
Locator.hover
Locator.inner_html
Locator.inner_text
Locator.input_value
Locator.is_checked
Locator.is_disabled
Locator.is_editable
Locator.is_enabled
Locator.is_hidden
Locator.is_visible
Locator.locator
Locator.nth
Locator.or_
Locator.press
Locator.screenshot
Locator.scroll_into_view_if_needed
Locator.select_option
Locator.select_text
Locator.set_checked
Locator.set_input_files
Locator.tap
Locator.text_content
Locator.type
Locator.uncheck
Locator.wait_for
```