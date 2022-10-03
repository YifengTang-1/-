# Form提交、Ajax提交

1、form 

https://www.w3school.com.cn/html/html_forms.asp

2、Ajax

http://www.jquerycn.cn/course/jquery-jquery-ajax-intro.html

## 区别

### 1、提交方式

form表单通常是通过在HTML中定义的action，method及submit来进行表单提交，另外也可以通过在js中调用submit函数来进行表单提交。

具体的提交方式有很多种，比如可以通过封装成XMLHttpRequest对象进行提交，

Ajax基于XMLHttpRequest进行的。

###  2、页面刷新 

Form提交，更新数据完成后，需要转到一个空白页面再对原页面进行提交后处理。哪怕是提交给自己本身的页面，也是需要刷新的，因此局限性很大。

Ajax 可以实现页面的局部刷新，整个页面不会刷新。

###  3、请求由谁来提交 

Form提交是浏览器完成的，无论浏览器是否开启JS，都可以提交表单。

Ajax 是通过js来提交请求，请求与响应均由js引擎来处理，因此不启用JS的浏览器，无法完成该操作。

###  4、是否可以上传文件 

最初，ajax出于安全性考虑，不能对文件进行操作，所以就不能通过ajax来实现文件上传，但是通过隐藏form提交则可以实现这个功能，所以这也是用隐藏form提交的主要用途。

后来XMLHttpRequest引入了FormData类型，使得通过Ajax也可以实现文件上传

参考

[csdn]: https://blog.csdn.net/weixin_30532973/article/details/97228190?spm=1001.2101.3001.6650.2&amp;utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7ECTRLIST%7ERate-2-97228190-blog-78641124.pc_relevant_3mothn_strategy_and_data_recovery&amp;depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7ECTRLIST%7ERate-2-97228190-blog-78641124.pc_relevant_3mothn_strategy_and_data_recovery&amp;utm_relevant_index=4

