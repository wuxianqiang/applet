# applet
微信小程序

## 基础
1. app.js
* `onLaunch`方法页面初始时候被执行
* 如果你想在多个地方都调用同一个方法，就可以写到app.js里面

2. app.json
* 每个页面js文件和wxml这两个文就是必须，其他文件可选
* 小程序的全局配置
* 如果小程序其它页面配置了就会覆盖调全局的
* `pages`对象配置小程序有哪几个页面
* `window`对象配置窗口的属性，背景颜色只能是黑白

3. app.wxss
* 全局样式，就是在项目的任何一个地方都可以用

4. pages文件夹

5. 其他
* `view`标签相当于html里面的`div`
* `onLoad`方法当页面加载完成执行
