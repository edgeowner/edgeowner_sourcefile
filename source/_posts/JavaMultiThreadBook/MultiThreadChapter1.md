---
title: Chapter(1)
tags: [多线程]
copyright: true
date: 2016-05-01 12:20:43
updated: 2016-05-01 20:19:21
categories: Java Multi-thread Programming书籍
mathjax: true 
---

### Thread类中start()方法和run()方法的区别
1. Thread.java类中的start()方法通知“线程规划器”，此线程已经准备就绪，等待调用线程对象的run()方法。这个过程其实就是让系统安排一个时间来调用Thread中的run()方法，也就是使线程得到运行，启动线程，具有异步执行的效果。
2. 如果代码调用thread.run()方法就不是异步执行，而是同步，那么此线程对象并不交给“线程规划器”来进行处理，而是由main()主线程来调用run()方法，也就是必须等run()方法中的代码执行完后才可以执行后面的代码。
3. ([<font color=#ff6600>代码Demo地址</font>](https://github.com/edgeowner/JavaMulti-threadProgramming))：参见com.multithread.demo.chapter1.ThreadShareDemo目录下代码

<!--more-->

-------




