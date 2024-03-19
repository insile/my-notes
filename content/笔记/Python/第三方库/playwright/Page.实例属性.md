##### Page.实例属性
```python
Page.mouse
	# 返回 Mouse 实例
Page.keyboard
	# 返回 Keyboard 实例
Page.touchscreen
	# 返回 Touchscreen 实例

Page.url
	# 返回 url
Page.video
	# 与此页关联的视频对象。返回 Video 实例
Page.is_closed
	# 页面关闭判断。返回 bool
Page.viewport_size
	# 视窗大小。Dict[width, height]
Page.context
	# 获取页所属的浏览器上下文。返回 BrowserContext 实例
Page.frames
	# 获取当前页面中的所有框架。返回 List[Frame]
Page.main_frame
	# 页面的主框架。返回 Frame 实例

Page.request
	# 与此页关联的 API 测试助手。返回 APIRequestContext 实例
Page.workers
	# 此方法返回与该页关联的所有专用 WebWorkers。返回 List[Worker]
```