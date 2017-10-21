# applet
微信小程序

## 基础
1. app.js
* 全局配置`js`文件里面必须要有一个App({})来初始化小程序
* `onLaunch`方法页面初始时候被执行
* `onShow`方法表示小程序显示的时候执行
* `onHide`方法表示在小程序隐藏的时候执行，如进入后台
* 如果你想在多个地方都调用同一个方法，就可以写到app.js里面

2. app.json全局配置
* 每个页面`js`文件和`wxml`这两个文就是必须，其他文件可选
* 小程序的全局配置
* 如果小程序其它页面配置了就会覆盖调全局的
* `pages`对象配置小程序有哪几个页面，文件名可以不加后缀，第一个表示首页
* `window`对象配置窗口的属性，背景颜色只能是黑白
* `tabBar` 导航栏，2~5个，接收list是一个数组，数组的每一项是一个对象

3. app.wxss全局样式
* 全局样式，就是在项目的任何一个地方都可以用

4. pages文件夹
* 其他页面`js`文件里面必须要有Page({})表示初始化来初始化页面

5. 其他
* `view`标签相当于html里面的`div`
* `onLoad`方法当页面加载完成执行
