## 说明
这是一个[uniapp](https://uniapp.dcloud.io/)项目，基于Vue 2.0 动画效果，运行流畅！
通常用于列表页面以及需要隐藏展示按钮的页面等，它带有右侧按钮展出与收起的动画，既可以给用户一个友好的点击体验，又可以避免遮挡用户视线。

## 源码地址
GitHub地址：[https://github.com/MichelleWangMX/wm-list-add](https://github.com/MichelleWangMX/wm-list-add)
uni-app插件市场地址：[https://ext.dcloud.net.cn/plugin?id=4131#detail](https://ext.dcloud.net.cn/plugin?id=4131#detail)

## 效果预览
![](https://ftp.bmp.ovh/imgs/2021/02/9d9b17da8190d96e.gif)

## 用法示例

```html
		<wm-list-add ref="add" @clickAdd="clickAdd"/>
```

```js
	import wmListAdd from '@/components/wm-list-add/wm-list-add';
export default {
	components: {
			wmListAdd
	},
	methods: {
			clickAdd(){
				console.log('点击加号执行操作')
			}
}
```
	
## 组件参数
|  属性名   | 类型  | 默认值  | 说明  |
|  ----  | ----  | ----  | ----  |
| bgColor  | `String` | #5094f2 | 默认背景颜色 |
| font-color  | `String` | #ffffff | 文字颜色 |
| isOpen  | `Boolean` | false | 默认是否关闭动画 |
| clickAdd | `Function` |   | 加号点击后的回调  |


## 组件方法
|  方法名   |  说明  | 方法参数 |  注  |
|  ----  | ----  | ----  | ----  |
| init()  |  初始化按钮状态  | 无 | 此方法会将按钮初始化至点击前的状态 |
| closeAnimation()  |  关闭右侧按钮  | `Function` | 此方法会关闭右侧按钮 |
| rotateAndScaleThenTranslate()  |  展开右侧按钮  | `Function` | 此方法会展开右侧按钮 |


## 谢谢
