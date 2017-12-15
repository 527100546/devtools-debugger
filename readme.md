# devtools-debugger

## Install 安装

```
	npm install devtools-debugger
```


## 使用方法

```html
<script src="node_modules/devtools-detect/index.js"></script>
<script>
	// check if it's open
	console.log('工具栏打开状态', window.devtools.open);
	// check it's orientation, null if not open
	console.log('工具栏方向', window.devtools.orientation);

	window.addEventListener('devtoolschange', function (e) {
		console.log('工具栏打开状态?', e.detail.open);
		console.log('工具栏打开状态?', e.detail.orientation);
	});
</script>
```


## Support

- Chrome DevTools
- Safari DevTools
- Firefox DevTools
- Opera DevTools
- Firebug
- Firebug Lite
