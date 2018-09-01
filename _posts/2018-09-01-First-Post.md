---
layout: post
title:  "First Post!"
date:   2018-09-01 18:05:55 +0800
categories: markdown
---
## 插入图片:
```markdown
![图注]({{ site.url }}/assets/imgs/bg.jpg)
```
![图注]({{ site.url }}/assets/imgs/bg.jpg)  
## 超链接 或文档。
```markdown
连接 [下载上图]({{ site.url }}/assets/imgs/bg.jpg). 
```
连接 [下载上图]({{ site.url }}/assets/imgs/bg.jpg).   
## 代码高亮
---
代码高亮  
```java
public class Hello{
    private String name;
    public static void main(String ... args) {
        System.out.println("Hello World");
    }
}
```
## 到行号的代码高亮
{% highlight java linenos %}
public class Hello{
    private String name;
    public static void main(String ... args) {
        System.out.println("Hello World");
    }
}
{% endhighlight %}

---
## 博客列表：  
{% for post in site.posts %}
+ [{{ post.title }}]({{ post.url }})
{% endfor %}
---
## 博客摘要列表  
{% for post in site.posts %}
1. [{{ post.title }}]({{ post.url }})
    1. {{ post.excerpt }}
{% endfor %}

