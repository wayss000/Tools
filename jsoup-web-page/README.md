## 说明

### 项目目标
利用爬虫访问CSDN博客，使访问量增加。

目标：使访问量低于1000的博客，访问量增加到1001；

### 实现思路

#### CSDN博客访问量增加的原理
CSDN博客通过HTTP访问一次即视为一次浏览，每两次浏览之间，时间需要大于60s；

#### jsoup提供的功能
jsoup提供了Java爬虫常用的API使用起来非常方便，具体教程：https://www.yiibai.com/jsoup/jsoup-quick-start.html

Jsoup官方API使用方法：https://try.jsoup.org/

#### 代码开发思路

1. 利用jsoup的实现爬虫，遍历博客主页
2. 遍历每一页，获取每篇博客的url和访问量，记录访问量低于1000+的
3. 对访问量低于1000的博客，利用爬虫程序模拟访问，最终达到阅读量大于1000的目录


#### 参考博文

**注意：** 以下两篇博客的已经不能运行了，原因是CSDN博客部分元素的CSS样式已经发生变化，但这两篇博客的思路非常值得参考和学习。

JAVA爬虫挖取CSDN博客文章(续)：https://blog.csdn.net/zhang5476499/article/details/54948348

Java的 jsoup使用之抓取CSDN个人博客内容：https://blog.csdn.net/hzp666/article/details/79098321