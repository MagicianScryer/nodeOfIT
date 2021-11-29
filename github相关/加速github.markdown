# 为了解决 github 在陆内加载过慢的问题

# 该文章也是用于熟悉 markdown 语法的笔记

## 导致 github 加载慢的原因

> 我们访问的是国外的 ip 地址

    打开cmd ping github.com
    会发现请求超时无法获取

## 解决办法（一定要按照步骤去解决）

- 打开此网站[dns 解析器](http://tool.chinaz.com/dns)
- 在 dns 搜索中直接搜索 github.com,找到 TTL 值最小的 IP 地址复制
- 在我的电脑中找到 C:\Windows\System32\drivers\etc 的路径打开 hosts 这个文件用笔记本(如果无法修改是权限不够，自行提权)
- 在最后一行加上该 ip 地址 和 github.com 如图所示

![avatar](https://img-blog.csdnimg.cn/20190423101513969.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyNzUwMjQw,size_16,color_FFFFFF,t_70)
