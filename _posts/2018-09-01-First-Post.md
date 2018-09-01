---
layout: post
title:  "First Post!"
date:   2018-09-01 18:05:55 +0800
categories: jekyll update
---
… 从下面的截图可以看到：
![有帮助的截图]({{ site.url }}/assets/imgs/bg.jpg)  
…你可以直接 [下载上图]({{ site.url }}/assets/imgs/bg.jpg).   

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

{% highlight java linenos %}
public class Hello{
    private String name;
    public static void main(String ... args) {
        System.out.println("Hello World");
    }
}
{% endhighlight %}

---
博客列表：  
{% for post in site.posts %}
+ [{{ post.title }}]({{ post.url }})
{% endfor %}
---
博客摘要列表  
{% for post in site.posts %}
1. [{{ post.title }}]({{ post.url }})
    1. {{ post.excerpt }}
{% endfor %}

