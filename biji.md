# 颜色渐变和透明度
## 颜色的透明度
1.  rgba()    **a** 代表的是透明通道，取值范围0-1
    `通过改变整体容器的透明度来实现透明，但是他会影响容器里面的内容`


  1.1 opacity:0~1
    filter:alpha(opacity:0~100)

2.   background:transparent  可以直接使用该值，实现完全透明
3.   HSL模式 色彩模式是工业街的一种颜色标准，H 色调（0-360）   S饱和度（百分比）  L亮度（百分比）
     HSLA模式 A表示透明度
     background-color:hsl(120,65%,75%);
     background-color:hsl(120,65%,75%，0.5);
#    图片格式
     png  ->无损压缩格式,ie6不支持png
     jpg  ->有损压缩格式
     GIF  ->动态图片
## 渐变
###  线性渐变  background:linear-gradient(to right,red,blue);  默认的渐变方向从上到下
    eg:
    background:linear-gradient(red 0%,blue 10%,green 70%,yellow);
    background:linear-gradient(10deg,red 0%,blue 10%,green 70%,yellow);  设置渐变的角度
    **通过关键字的方式（to left/top/left top）或者角度（10deg）的方式来设置渐变的方向** 
###  径向渐变  background:radial-gradient(red,green,orange,yellow);
  1. background:radial-gradient(red,green,blue);
  2. circle 代表圆形， 100px代表渐变的区间，at代表渐变起始位置
    background:radial-gradient(circle,red 30%, green 50%, blue);  径向渐变的范围100px之内
    background:radial-gradient(circle 50px  at 20px 50px , red 0%,green 50%,blue);
    ellipse 代表椭圆，椭圆的大小需要两个半径作为约束
    background:radial-gradient(ellipse 50px 30px at 120px 120px,red,blue,green);
###  重复渐变
    background:repeating-radial-gradient(ellipse 50px 30px at 120px 120px,red,blue,green);
   
###  css3的新增选择器
    @media响应式   12栅格化   less    nodejs   @keyframes（创建动画）   @font-face(自己去指定字体)
    
#html5    
      html头部声明：通知浏览器以什么样的标准解析html
      html5简写了头部声明

    多媒体播放，剪辑软件
    **音频和视频的处理 **
    画布canvas
    事件  移动端事件 touchstart touchend touchmove
##html5概述
新版的html，html5的诞生，包含的功能，哪些浏览器支持，哪些不支持
#html5新增标签  向下兼容，能够识别html4的语法
语法规则：
        标签要小写
        属性值不加""或''
        可以省略某些标签
            -html body head tbody 
        单标签不用加结束标签
        --img input
        废除的标签
        -font center big
        新添加的标签
        -header footer nav  从布局的层面来说和之前的没有区别
        语义化标签：有特殊和意义的标签
        seo   Search Engine Optimization缩写     搜索引擎优化
##SEO 搜索引擎优化
    搜索引擎规则，算法
    语义化是让搜索引擎看的
##sem 搜索引擎营销
##html5的新特性
    用于绘画的canvas元素
    用于媒介回放的 video 和 audio 元素
    对本地离线存储的更好的支持
    新的特殊内容元素，比如 article、footer、header、nav、section、hgroup、aside、
    新的表单控件，比如 calendar、date、time、email、url、search
### 结构性标签 
### 块级标签 
### 行内标签
 meter progress time 
### 多媒体标签 video audio
### 列表标签
### 交互性标签(仅做了解)
    --menu
    --command
### html5表单
    表单的结构更自由
    新增表单控件 
         email  
         url(网址) 
         date(日历)  month datatime datatime-local week
         number 
         range(滑块)
         search
         color(拾色器)   
         pattern(正则) 
         autofocus(自动聚焦)值为autofocus [不能同时获得多个焦点，]   
         list【关联】(不常用)

    验证属性：
        autocomplete（自动完成）
        placeholder(默认值)只用于email？？？
        require(必填)
    最大值，最小值，固定值
        min max step
    表单属性：
        novalinated  

    例子：

            eg:
            <form action="">
            email:
            <input type="email" name = "email" required><br/>
            <input type="submit">
            </form>
##验证方式
选择器： 动态的判断表单是否符合验证
input:valid{
    color:red;   //符合验证的变为红色
}
input:invalid{
    color:green;   //没有符合验证的变为绿色
}



表单验证插件
jquery-validate
也可以在github上搜索到

提示信息为中文 修改源码  messages 


作业：
表单的验证
机器猫






      
    
    




















