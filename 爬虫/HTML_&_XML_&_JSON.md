# 什么是超文本标记语言(HTML)

Hyper Text Makeup Language  ->HTML
它包括一系列标签．通过这些标签可以将网络上的文档格式统一，使分散的Internet资源连接为一个逻辑整体  
使用HTML，将所需要表达的信息按某种规则写成HTML文件，
通过专用的浏览器来识别，并将这些HTML文件“翻译”成可以识别的信息，即现在所见到的网页
浏览器<-->服务器

# 什么是http协议（超文本传输协议）

超文本传输协议（Hypertext Transfer Protocol，HTTP）是一个简单的请求-响应协议，它通常运行在TCP之上。它指定了客户端可能发送给服务器什么样的消息以及得到什么样的响应。  
HTTP协议是Hyper Text Transfer Protocol（超文本传输协议）的缩写,是用于从**万维网（WWW:World Wide Web ）服务器**传输**超文本**到**本地浏览器**的传送协议。
HTTP是一个基于TCP/IP通信协议来传递数据（HTML 文件, 图片文件, 查询结果等）。
浏览器显示的内容都有 `HTML`、`XML`、`GIF`、`Flash` 等，浏览器是通过 MIME Type 区分它们，决定用什么内容什么形式来显示。  
注释：MIME Type 是该资源的媒体类型，MIME Type 不是个人指定的，是经过互联网（IETF）组织协商，以 RFC（是一系列以编号排定的文件，几乎所有的互联网标准都有收录在其中） 的形式作为建议的标准发布在网上的，大多数的 Web 服务器和用户代理都会支持这个规范   
**媒体类型通常通过 HTTP 协议，由 Web 服务器告知浏览器的，更准确地说，是通过 Content-Type 来表示的。例如：Content-Type：text/HTML。**  

## http工作原理

HTTP协议工作于客户端-服务端架构上。  
浏览器作为**HTTP客户端**通过**URL**向**HTTP服务端**即**WEB服务器**发送所有请求。  
Web服务器有：Apache服务器，IIS服务器（Internet Information Services）等。  
 
典型的HTTP事务处理有如下的过程：
（1）客户与服务器建立连接；
（2）客户向服务器提出请求；
（3）服务器接受请求，并根据请求返回相应的文件作为应答；
（4）客户与服务器关闭连接。

## http通信协议流程

Web Browser  <--> HTTP server <--> CGI program <--> Database

# 什么是可扩展标记语言(XML)

可扩展标记语言（标准通用标记语言下的一个子集、外语缩写：XML），又称可扩展置标语言，是一种标记语言。置标指电脑所能理解的信息符号，通过此种标记，电脑之间可以处理包含各种信息的文章等。
它可以用来标记数据、定义数据类型，是一种允许用户对自己的标记语言进行定义的源语言。 它非常适合万维网传输，提供统一的方法来描述和交换独立于应用程序或供应商的结构化数据。是Internet环境中跨平台的、依赖于内容的技术，也是当今处理分布式结构信息的有效工具。
## XML和HTML
XML有两个先驱：SGML和HTML，这两个语言都是非常成功的标记语言，但是都有一些与生俱来的缺陷。XML正是为了解决它们的不足而诞生的。  

+ SGML
  
早在Web未发明之前，SGML(Standard Generalized Markup Language，标准通用标记语言)就已存在SGML具有非常复杂的文档结构，主要用于大量高度结构化数据的访问和其他各种工业领域，在分类和索引数据中非常有用。
虽然SGML的功能很强大，但是它不适用于Web数据描述，而且SGML软件的价格非常昂贵；另外，SGML十分庞大，既不容易学，又不容易使用，在计算机上实现也十分困难：不仅如此，几个主要的浏览器厂商都明确拒绝支持SGML，这无疑是SGML在网上传播遇到的最大障碍。鉴于这些因素，Web的发明者发明并推出了HTML。 

+ HTML
  
1989年，HTML诞生，它抛弃了SGML复杂庞大的缺点，继承了SGML的很多优点。HTML最大的特点是简单性和跨平台性。正是由于HTML的简单性，使得基于HTML的Web应用得到了极大的发展。 

+ XML的产生

随着Web应用的不断发展，HTML的局限性也越来越明显地显现了出来，如HTML无法描述数据、可读性差、搜索时间长等。人们又把目光转向SGML，再次改造SGML使之适应现在的网络需求。随着先辈的努力，XML诞生了。  
当前的一些网站内容建设者们已经开始开发各种各样的XML扩展，比如**数学标记语言MathML**、化学标记语言CML等。


# 什么是 JSON(JavaScript Object Notation, JS 对象简谱) 

是一种轻量级的**数据交换格式**。它基于 ECMAScript (欧洲计算机协会制定的js规范)的一个子集，采用*完全独立于编程语言的文本格式来存储和表示数据*。简洁和清晰的层次结构使得 JSON 成为**理想的数据交换语言**。 易于人阅读和编写，同时也易于机器解析和生成，并有效地提升网络传输效率。

## JSON和XML

可以看到，JSON 简单的语法格式和清晰的层次结构明显要比 XML 容易阅读，并且在数据交换方面，由于 JSON 所使用的字符要比 XML 少得多，可以大大节约传输数据所占用的带宽。  
JSON格式取代了xml给网络传输带来了很大的便利,但是却没有了xml的一目了然,尤其是json数据很长的时候,我们会陷入繁琐复杂的数据节点查找中。

## 记录一下在vscode上面html的环境配置

首先创建一个`.html`文件
可以快捷创建,首先使用一个英文`!`然后出现选项之后回车即可，
实际上出现问题，没有办法进行快捷创建，如何改进，
在vscode中选择右下角，有一个`Select Language Mode`来选择语言，换成html即可快捷创建  
又出现问题，不知道怎么让html文件直接在浏览器中显示，解决办法是
在vscode中`ctrl+shift+p`快捷键，进入命令面板，然后找到`live sever`点击，即可看到右下角出现`Go Live`点击即可使用浏览器查看你编辑的html文件

# HTML简单制作网页

HTML标签 通常是成对出现的 <head> </head>  
单标记元素  
<!--注释-->

