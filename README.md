# ArUI-Progress
一根非常简单的进度条

# 准备

必要模块：Bootstrap CSS，FontAwsome
```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.6.0/dist/css/bootstrap.css">
<link href="https://cdn.bootcdn.net/ajax/libs/font-awesome/5.15.3/css/all.css" rel="stylesheet">
```
引入ArUI-Progress js与css：

```html
<link href="https://cdn.jsdelivr.net/gh/ArSrNa/ArUI-Progress/arloading.css" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/gh/ArSrNa/ArUI-Progress/arloading.js"></script>
```

# 使用

首先在div里创建一个div，包含id

`<div id="test"></div>`

然后执行函数

```JavaScript
arLoading({
	text:'Ar-Sr-Na SAO-Serverless Automatic Organization',
	color: '#DDDDDD',
	id: 'test'
	size: '3',
	icon: 'fa-info-circle'})
```

其中：

| 字段  | 类型          | 描述                                                                                           | 注意                 | 默认值               |                |
|-------|---------------|------------------------------------------------------------------------------------------------|----------------------|----------------------|----------------|
| text  | String        | 显示的文本，可以使用html格式，例如"我永远喜欢御坂美琴"或"我永远喜欢御坂美琴<br>其他都是我小号" | 内置了<h5>标签       | /                    |                |
| color | String        | 背景颜色，支持css格式                                                                          | 例如white或#66CCFF   | white                |                |
| id    | String        | 创建进度条的控件id                                                                             | 仅支持DIV            | /                    |                |
| size  | number/String | 图标大小                                                                                       | Fontawsome的fa-*x    | 3                    |                |
| icon  | String        | 图标                                                                                           | Fontawsome的fa-xxxxx | 仅支持FontAwsome图标 | fa-info-circle |

# example

```html
<div id='test'></div>
<link rel="stylesheet" href="arloading.css">
<script src="arloading.js"></script>
<script>
arLoading({
	text:'Ar-Sr-Na SAO-Serverless Automatic Organization',
	color: '#DDDDDD',
	id:'test'})
</script>
```

## Powered By Ar-Sr-Na 云计算项目团队