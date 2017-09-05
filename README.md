# phantomQuery
>> 本项目主要基于PhantomJS实现多线程多功能化的采集需求.

## 主要包含了以下类别的功能:
* 页面与数据采集
* Dom操作
* 屏幕捕获(png|pdf)
* 性能分析
* 运行自定义js脚本或命令

### 页面与数据采集

* 通过PhantomJS无头浏览器加载网页
* 查看详细的响应数据，包括页面内容，标题，状态代码等。
* 处理重定向|视窗设置|渲染时间|页面延迟
* 查看javascript控制台错误(该项常用于页面加载完成后的console.log()输出)
* 

### Dom操作
* 元素选择器-$("p#demo")
* 获得|设置内容 - text()、html() 以及 val()
* 获取|设置属性 - attr()
* 添加元素或内容 - append()、prepend()、after()、before()
* 删除元素或内容 - remove()、empty()
* 遍历|祖先|同胞|后代|过滤 - 、add()、children()、closest()、each()、end()、eq()、find()、first()、last()、map()、next()、nextAll()、parent()
* 包裹|替换 - wrap()、wrapAll()、replaceWith()、replaceAll()


### 屏幕捕获(png|pdf)

* 浏览器视窗大小|尺寸|边距|指定x,y|width|height|background
* pdf文件的固定页眉和页脚
* 截图生成指定尺寸或比例大小并同步至远程OSS

### 性能分析

* 调试日志
* 缓存处理
* 网络请求及其相应列表

### 运行自定义js脚本或命令

* PhantomJS支持的自带命令
* 载入自定义js脚本
  * 资源超时处理时
  * 请求指定资源时
  * 收到资源响应时
  * 处理页面错误时
  * 打开页面时
  * 载入完成时