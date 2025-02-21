---
{"dg-publish":true,"permalink":"/05publishedweb/W002-学习进度/250118_-1_进度搬运_FreeRTOS和RT-Thread和python爬虫/","noteIcon":"","created":"2025-02-21T21:51:50.695+08:00","updated":"2025-02-21T22:02:42.871+08:00"}
---




> [!关于本篇：]
> 本篇内容搬运自QQ空间：https://user.qzone.qq.com/1312201038/main
> 仅用于存档和记录学习进度，若有视频(及其截屏)，请以空间为准
> 

*记录时间：2025年01月18日*

250118：进度：RTOS。已完成：FreeRTOS、RT-Thread  
其实RTOS就是一个极简的、运行在单片机上面的操作系统，它解决了两个单片机开发的难点问题。一是通过内核解决了单一芯片中的硬件层、驱动层、内核、软件层、应用层纯手敲工程量巨大的问题。二是通过环形单链表结构的软件模拟线程、任务优先级、中断嵌套函数和回调函数，解决了单核SoC无法实现多线程的问题。不过相比之下，freeRTOS似乎只是一个更“纯粹”的内核（可移植性更高），在同样代码量的情况下占用极小，但相对应的功能和生态明显不如RT-Thread。在开发的时候就能明显感觉出来，使用RT-Thread开发明显更为“优雅”，需要什么外设或者系统级驱动，直接点点点就能装上去，而代价就是：同样的图中，一个调用两个定时器（一个动态一个静态）实现简单的多线程定时器控制的代码，freeRTOS中只占用11-35KB的Flash，而RT-Thread竟然直接干上52.8KB了！不过不得不说，国内嵌入式也是好起来了。  
另外小小的记录一下这个学期无聊之时，为了打发时间做的两个小项目，都是python的，均已上传到github：  
一个是优雅存储X岛的小说串的脚本（其实就是一个爬虫，不过做了访问限制，别天天霍霍人家服务器）： [https://github.com/chencxt/nmbxdSpider](https://github.com/chencxt/nmbxdSpider)   
另一个是这两天我正在给电脑做维护，重装系统发现忘记备份浏览器书签了。所以我就在想，有没有可以优雅地实现自动化备份浏览器书签的插件呢？一番折腾之下，利用win的开机自启动，简单做了一个全自动把chrome的书签导出为HTML（方便导回）的脚本。只需要按照说明，适配一下电脑就可以了： [https://github.com/chencxt/bookmark2html](https://github.com/chencxt/bookmark2html)   
那么，继续分享笔记和开源代码吧：链接:  [https://pan.baidu.com/s/116eq1ZxKnP2WYtPWoCkjdw?pwd=978d](https://pan.baidu.com/s/116eq1ZxKnP2WYtPWoCkjdw?pwd=978d)  提取码: 978d 复制这段内容后打开百度网盘手机App，操作更方便哦  
--来自百度网盘超级会员v6的分享



![attachment/250118-1 1.jpeg](/img/user/05publishedweb/W002-%E5%AD%A6%E4%B9%A0%E8%BF%9B%E5%BA%A6/attachment/250118-1%201.jpeg)

![attachment/250118-2 1.jpeg](/img/user/05publishedweb/W002-%E5%AD%A6%E4%B9%A0%E8%BF%9B%E5%BA%A6/attachment/250118-2%201.jpeg)