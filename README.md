# android_listview
android下拉更新，上拉加载更多的简单listview

最近做数据绑定控件，需要包含刷新和加载分页的listview；网上的代码量太大，所以就参考了下一些实现方法，写了一个，目前测试下来，还是可以的，给大家分享下。

实现原理：
重写onTouchEvent事件，判断手势，编写上拉下拉触发事件。

上拉下拉时，控制headerview和footerview 距离头部和底部的padding来实现的。

需要隐藏时设置padding为负的headerview高度

需要显示时设置padding为实际padding即可
