## 1ibrary-front-end
> 一图app前端代码
## 时间轴

### 17.04.08
创建项目，编写NavigationBar组件,ShareNav组件。
编写网络请求工具库HttpUtils.js

###  17.04.09
- 编写底部标签BottomTabs组件     
- 编写带有搜索栏的导航SearchNav组件    
- 编写首页的主体部分，即书目列表的ListView实现
- todo: 网络请求部分的代码还没有写（下拉刷新的实现）。       
接下来需要解决的分别是
- 搜索提示页
- 搜索结果页。     
  
### 17.04.10
- 完成搜索历史&推荐页
- 熟悉本地存储技术点AsyncStorage    

待做:    
- 搜索结果页

### 17.04.11
- 完成搜索提示页
- 完成搜索结果页除ScrollableBar之外的部分
待做:    
- 搜索结果页
- 抽象出BookList组件，将BookItem设置为自定义    
后续思路:     
- 在每个BookItem上设定navigator组件，实现BookItem和Book详情页面的跳转

### 17.04.12
> 今天一图这块啥也没干，晚上收到了新的设计稿，变漂亮了，大概想了一下构建，思路上没有很大的出入。
> 明天开始动工！^_^ 加油！💪

### 17.04.13
- 对之前做的四个页面进行了新设计稿的改版
- 明天要做的图书详情页思路：先分页面把每个页面实现，然后用navigator实现页面间跳转
- 出现的问题:ScrollableTabView组件不够灵活，暂时放弃自定义，后期如果有时间再补救

### 17.04.14
- 改版顶部导航样式
- 完成图书详情页的基本布局

### 17.04.15
- 完成首页部分的所有单个页面的布局和事件的编写
- 利用navigator实现页面之间的跳转

### 17.04.16
- 完成书单的增加和删除部分
- bug: 书单这部分本来打算使用ListView这个组件，但当data改变的时候,ListView并没有变化，不得已最后使用了ScrollView然后map，这个以后需要留意，现在暂时没搞明白怎么回事

### 17.04.17
>可以说是非常拼的一天了。。。。     

- 剩下登录页的两个页面没写
- 剩下个人页面的setting页和aboutus页没写

> 连写带改连续弄了8h。。。。。眼睛可以说是非常痛了。。。。😂
> 现在去躺尸。。。。。。

- 大boss: 网络层请求部分的代码 最后写
- 大boss: 排除所有的warning 网络层之前做 用chrome dev调试定位

### 17.04.20
- 完成所有页面布局
- 明天测试网络层

### 17.04.23
- 网络层局部测试成功
待做:    
- 所有网络层请求代码
- listview上拉刷新使用refreshcontrol来做，下拉加载参考[这篇回答](https://segmentfault.com/q/1010000004101829)
- 首页要做缓存 一开始先显示缓存 然后加载成功再刷新 书单在网络请求结束之后也要本地缓存
- 细节部分怎么完善？用户提示怎么做，用户不存在这些，统统暂时alert
- warning边做边排了一部分，集中排除要在最后
- 真机调试

### 17.04.24
- 图书列表页面网络请求完成 图片无法加载
- 加入书单部分的圆圈面积比较小不太好点 