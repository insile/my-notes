##### class APIResponse
- `APIResponse.说明`
	- 响应
- `APIResponse.实例属性`
```python
APIResponse.body
	# 返回包含响应体的缓冲区。bytes
APIResponse.dispose
	# 释放此响应的主体。如果不调用，主体将保留在内存中，直到上下文关闭。
APIResponse.json
	# 返回响应体的 JSON 表示形式。Serializable
	# 如果响应主体不能通过.JSON.parse 进行解析，则此方法将抛出异常
APIResponse.text
	# 返回响应体的文本表示形式。str
```
- `APIResponse.实例方法`
```python
APIResponse.headers
	# HTTP 标头
APIResponse.headers_array
	# HTTP 标头的数组
APIResponse.ok
	# 包含一个布尔值，说明响应是否成功(状态在200-299范围内)。
APIResponse.status
	# 包含响应的状态代码(例如，200表示成功)。
APIResponse.status_text
	# 包含响应的状态文本(例如，通常是“ OK”表示成功)。
APIResponse.url
	# 包含响应的 URL。
```
