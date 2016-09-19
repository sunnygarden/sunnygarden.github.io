---
layout: post
title: "Markdown快速入门"
tags: [useful utils]
categories: [utils]
---


　　刚接触Markdown，总结一些常用语法，希望能帮助一些像我一样的初学者快速入门。
　　
####一、段落前面的空格

输入法切换到全角，敲两次空格键

###二、换行

敲两次回车

###三、层级标题

在前面加#，#越多，字越小

例如：

    #一级标题
    ##二级标题
    ###三级标题
    ####四级标题
    #####五级标题

效果如下：


#一级标题
##二级标题
###三级标题
####四级标题
#####五级标题

 
###四、层级引用

在前面加>, >越多，层级嵌套越深（注意>后面的空格不要忘了）

例1：
    > MarkDown的引用只需在前面加上>就可以了，非常简单，你也可以试试
    
效果如下：

> MarkDown的引用只需在前面加上>就可以了，非常简单，你也可以试试
 
例2：

    > 这是一级引用
    >> 这是二级引用
    >>> 这是三级引用
    >> 回到二级引用
    
    > 回到一级引用
    
效果如下：
> 这是一级引用
>> 这是二级引用
>>> 这是三级引用
>> 回到二级引用

> 回到一级引用	 

引用的块内也可以使用其他MarkDown语法：

    > ## 标题
    >> * 这是第一行列表项。
    >> * 这是第二行列表项。
    >>> 示例代码：
    >> > 
    ```
    System.out.println("Hello World!");
    ```

显示效果：

> ## 标题
>> * 这是第一行列表项。
>> * 这是第二行列表项。
>>> 示例代码：
>> > 
```
System.out.println("Hello World!");
``` 


###五、列表项目

（1）	无序列表：列表标记：*、+或-（标记符后记得加上空格）

例如：

```
* 无序列表1
+ 无序列表2
- 无序列表3
```

效果样式：

* 无序列表1
+ 无序列表2
- 无序列表3


（2）	有序列表：数字接着一个英文句点

例如：

```
1. 有序列表1
2. 有序列表2
3. 有序列表3
```

效果样式：

1. 有序列表1
2. 有序列表2
3. 有序列表3


###六、代码块

方法一：将代码块放入```之间即可

输入：

    ```
    public class HelloWorld {
        public static void main(String[] args){
           System.out.println("Hello World!");
       }
    }
    ```
 
 
方法二：将每行文本前空四个空格（Markdown 会把自动将其转换为代码块）


        public class HelloWorld {
            public static void main(String[] args){
               System.out.println("Hello World!");
           }
        }

###七、强调(*和_的使用)

（1）	斜体强调的两种方式：

```
*斜体强调*    
_斜体强调_
```


效果样式：

*斜体强调*


（2）	粗体强调的两种方式：

```
**粗体强调**
__粗体强调__
```

效果样式：

**粗体强调**

   
（3）	斜体+粗体强调的两种方式：

```
***斜粗体强调***
___斜粗体强调___
```


效果样式：

***斜粗体强调***
 


###八、分割线：三个_短线

例如：

```
___

```

效果样式：

___


###九、网页连接或邮箱：

方法1：方括号内显示名称，圆括号内显示网址

 
例如：

```
[sunnygarden](http://sunnygarden.top)
```

效果样式：

[sunnygarden](http://sunnygarden.top)

 
方法2：尖括号内显示网址


例如：

```
<http://sunnygarden.top>
```

效果样式：

<http://sunnygarden.top>


方法3：http链接可直接显示网址：（邮箱链接不可用此方法）

例如：

```
大家好，欢迎访问我的blog地址：http://sunnygarden.top/
我的邮箱是：<wkuisky@163.com>
```

效果样式：


大家好，欢迎访问我的blog地址：http://sunnygarden.top/
我的邮箱是：<wkuisky@163.com>


###十、图片链接

（1）	内联图片


格式：

```
![alt text](/path/img.jpg)或![ alt text](/path/img.jpg “optional title”)
```

例1：图片链接失效：

```
![sunnygarden的logo](http:/a/b/c/logo.png  "logo")
```

效果样式：

 ![sunnygarden的logo](http:/a/b/c/logo.png  "logo")
 
例2：图片链接有效：

```
![sunnygarden的logo](https://raw.githubusercontent.com/sunnygarden/sunnygarden.github.io/master/favicon.ico)
```

效果样式：

![sunnygarden的logo](https://raw.githubusercontent.com/sunnygarden/sunnygarden.github.io/master/favicon.ico)


（2）	引用图片

格式：

```
![alt text][id]
[id]:url/img.jpg “optional title”
```

例如：

```
![logo][id]
[id]: https://raw.githubusercontent.com/sunnygarden/sunnygarden.github.io/master/favicon.ico
```

效果样式：

![logo][id]
[id]: https://raw.githubusercontent.com/sunnygarden/sunnygarden.github.io/master/favicon.ico 

###十一、表格

（1）无对齐方式的普通表格（默认左对齐）


例如：

```
First Header | Second Header | Third Header
------------ | ------------- | ------------
Content Cell | Content Cell | Content Cell
Content Cell | Content Cell | Content Cell
``` 

效果样式：

First Header | Second Header | Third Header
------------ | ------------- | ------------
Content Cell | Content Cell | Content Cell
Content Cell | Content Cell | Content Cell

（2）通过 : 来设置对齐样式

例如：

```
First Header | Second Header | Third Header
:-----------| :-----------: | -----------:
Left  | Center  | Right
Left  | Center  | Right
```

效果样式：


First Header | Second Header | Third Header
:-----------| :-----------: | -----------:
Left  | Center  | Right
Left  | Center  | Right
