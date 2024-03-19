##### class Mouse
- `Mouse.说明`
	- 鼠标相对于视口的左上角以主框架 CSS 像素操作。
	- 每个页面对象都有自己的鼠标，可以通过 [[Page.实例属性|page.Mouse]] 访问。
```python
# using ‘page.mouse’ to trace a 100x100 square.
page.mouse.move(0, 0)
page.mouse.down()
page.mouse.move(0, 100)
page.mouse.move(100, 100)
page.mouse.move(100, 0)
page.mouse.move(0, 0)
page.mouse.up()
```
- `Mouse.实例方法`
```python
page.click(x, y, button, click_count, delay)
	# 移动单击的快捷键
page.dblclick(x, y, button, click_count, delay)
	# 移动双击的快捷键

page.move(x, y)
	# 鼠标移动。
page.down(button, click_count)
	# 按下鼠标。
page.up(button, click_count)
	# 松开鼠标。
page.wheel(delta_x, delta_y)
	# 鼠标滚轮。

# x, y：相对于左上角屏幕坐标
# button：鼠标按键默认左键 "left"，"right"，"middle" 
# click_count：点击次数 
# delay：在 mousedown 和 mouseup 之间等待的时间
# delta_x, delta_y：水平垂直滚动像素
```