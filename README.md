# applet
微信小程序

## 基础
1. app.js
* 全局配置`js`文件里面必须要有一个App({})来初始化小程序
* `onLaunch`方法页面初始时候被执行
* `onShow`方法表示小程序显示的时候执行
* `onHide`方法表示在小程序隐藏的时候执行，如进入后台
* 如果你想在多个地方都调用同一个方法，就可以写到app.js里面
* globalData对象定义全局属性，在其他页面使用时候必须用getApp()获取一下

2. app.json全局配置
* 每个页面`js`文件和`wxml`这两个文就是必须，其他文件可选
* 小程序的全局配置
* 如果小程序其它页面配置了就会覆盖调全局的
* `pages`对象配置小程序有哪几个页面，文件名可以不加后缀，第一个表示首页
* `window`对象配置窗口的属性，背景颜色只能是黑白
* `tabBar` 导航栏，2~5个，接收list是一个数组，数组的每一项是一个对象
* `debug`属性可以是true和false表示是否输出日志

3. app.wxss全局样式
* 全局样式，就是在项目的任何一个地方都可以用

4. pages文件夹
* 其他页面`js`文件里面必须要有Page({})表示初始化来初始化页面

5. 其他
* `view`标签相当于html里面的`div`
* `onLoad`方法当页面加载完成执行
* `wx.navigateTo({url: '../index/index'})`定义路由，相当于js实现跳转
* `navigator`标签也可以实现跳转，url属性指定跳转到的页面
*  `wx.navigateBack()`方法返回这个页面
* 条件渲染，`wx:if="布尔值"` 这样写
* `hidden`也可以控制显示和隐藏，但是只作用于text标签上
* `wx:for="{{[id,5,4,3,2,1]}}"`循环可以这样写，当前项用`{{item}}`表示，可以用`wx:for-item`来更改变量的名字，下标用`{{index}}`表示，可以用`wx:for-index`来更改变量的名字
* `<template name="object"></template>`模板定义的时候要有name属性
* 使用的时候`<template is="object" data="{{data}}"></template>`

### 标签
1. `<view>` 相当于 `div`
2. `<text>` 相当于 `p`
3. `<image>` 相当于 `img`
4. `1rpx = 2px `
5. 宽度 `750rpx = 100%`
6. 线条使用 `1px`
7. 绑定点击事件 `bindtap`会冒泡 `catchtap`不会冒泡相当于 `click`
