#### Day1
* 基本依赖的安装和初始化
  - 安装并检测依赖，vuex,less,less-loader(less is ok)
  - 添加reset.css
  - mock安装、编写、测试
  - axios的编写和测试
  - 完成了一个简单的注册功能
![](https://raw.githubusercontent.com/dirstart/image_bed/master/last1.jpg)
  - 写完了一个简单的服务端程序，并且在本地启动，并在前端程序中加入proxyTable
![](https://raw.githubusercontent.com/dirstart/image_bed/master/last2.jpg)
  - 用postman这个工具验证了一下接口的正确性
![](https://raw.githubusercontent.com/dirstart/image_bed/master/last3.jpg)

#### Day2
* 线上部署准备
  - 购买阿里云学生套餐，半年内免费使用ECS和其他各种云服务
![](https://raw.githubusercontent.com/dirstart/image_bed/master/last4.jpg)
  - 给ECS配置Node和MongoDB环境
![](https://raw.githubusercontent.com/dirstart/image_bed/master/last5.jpg)
![](https://raw.githubusercontent.com/dirstart/image_bed/master/last6.jpg)

#### Day3
- 先做了首页的固定底部的地方，时间太敢，还没有做完。目前决定使用iconfont做，正在考虑是否使用svg。
![](https://raw.githubusercontent.com/dirstart/image_bed/master/last7.png)

#### Day4
- 代码优化，准备使用vue-router的beforeEach来做真正的登录功能。
- 添加NotFound的 demo 页面(后期有空则修改)。

#### Day5
- 处理iconfont的引入，本来是静态static在html里面引入，但是不符合webpack思想，百度了下如何正统地引入它
> 在html引用是很不干净的，因为这样webpack的压缩就压缩不到这里的`static css`了。
修改办法：引用之中使用 './' 等相对路径
信息来源：http://blog.csdn.net/xiaoermingn/article/details/53543001
- 新增`rem`移动端适配.
> 移动端布局的一些学习、思考和引入，主要为 `rem` 布局。
- less之间的相互引用
> @import './base.less'; // 这个是正确的格式，少个`;`均会报错
@import "~assets/css/ydui-reset"; // 这个是在 webpack 下的写法
- 全局采用`box-sizing`布局

#### Day6
- 由于时间缘故决定采用`Muse-UI`。

#### day7
- 真正的注册登录的session
> 使用session为了： 1.对于未登录的用户跳至某些页面进行拦截。（前后端都要拦截）
2.跳转某些页面需要带有用户信息

#### day8
- 略坑爹，muse-ui的icon有时候需要翻墙才能拿到图标。考虑一个个下载下来或者弄个vpn或者别人的cdn.
- 已引入CDN：@import 'https://cdn.bootcss.com/material-design-icons/3.0.1/iconfont/material-icons.css';
> https://www.2cto.com/kf/201707/658375.html

#### day9
- 写不完了，有点蛋疼。
- 新改页面头部
- 新改页面登录注册页，全用组件了，一个个样式自己调太慢了

#### day10
> 没时间写文档了。。。下面直接放图。。
![](https://raw.githubusercontent.com/dirstart/image_bed/master/last7.png)
![](https://raw.githubusercontent.com/dirstart/image_bed/master/last8.png)
![](https://raw.githubusercontent.com/dirstart/image_bed/master/last9.png)
![](https://raw.githubusercontent.com/dirstart/image_bed/master/last10.jpg)
![](https://raw.githubusercontent.com/dirstart/image_bed/master/last11.jpg)
![](https://raw.githubusercontent.com/dirstart/image_bed/master/last12.jpg)
![](https://raw.githubusercontent.com/dirstart/image_bed/master/last13.png)




