---
layout: post
title:  "React Native开发集锦"
date:   2018-03-10 16:36:21 +0100
categories: jekyll update
---

#### submit vs execute java
```    
public SubmitVsExecute() {
    System.out.println("");
    ExecutorService service = Executors.newFixedThreadPool(2);
    for (int i = 0; i < 2; i++) {
        int a = 4, b = 0;
        service.execute(new Runnable() {
            @Override
            public void run() {
                System.out.println(a / b);
                System.out.println("Thread name in runnable after divided 0" + Thread.currentThread().getName());
            }
        });
        service.shutdown();
    }
}

```
constructor() {
    this.state = {isReady: false};
}
```
* execute执行Runnable，submit执行Callable
* execute返回Void，submit返回Future
* execute执行的runnable发生异常的时候，外界不能catch，submit可以通过future.get感知到

#### 价格

真正的无中介费用，assignment/Homework的价格通常在90 USD以上，Exercise/Lab稍低。欢迎你货比三家。支持PayPal/支付宝/微信支付。

#### 联系

为了节省时间，方便报价，询问时麻烦附上你的年级和课程名，如：大二，Algorithm and Data Structure，作业要求请发送至byang7924@gmail.com，同时微信我：xxhh169


[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
