# add JavaScrpit-JS插件
* JSDemo
* JDMenu 京东无延迟菜单
* DatePicker组件开发
* 手风琴效果开发


## add-02
### JDMenu 京东无延迟菜单
#### 1.开发普通二级菜单

* 事件代理方式进行绑定
* `mouseenter`和`mouseover`的区别：
* 使用`mouseover/mouseout`时候，如果鼠标移动到子元素上，即便没有离开父元素，也会触发父元素的`mouseout`事件；
* 使用`mouseenter/mouseleave`时，如果鼠标没有离开父元素，在其子元素上任意移动，也不会触发`mouseleave`事件；

#### 2.加入延迟优化
* 切换子菜单的时候，用`setTimeout`设置延迟
* `debounce`去抖o((⊙﹏⊙))o.技术：
* 在事件被频繁触发时买只执行一次

#### 3.基于用户行为预测的切换技术

* 跟踪鼠标的移动
* 用鼠标当前位置，和鼠标上一次位置与子菜单上下边缘形成的三角区域进行比较

## add-03
### DatePicker组件开发
#### 1.基础页面制作

* 标头
* 身体

#### 2.数据部分

* 渲染当月日历表格
* 用于点击时取日期值

##### 日期对象

* `newDate(year,month-1,date)`
* 月份需要-1
* 越界自动进退位
* `getFullYear()/getMonth()/getDate()`
* `getDay()`获取当前日期是周几？
