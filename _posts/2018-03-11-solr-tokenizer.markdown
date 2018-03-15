---
layout: post
title:  "Solr文本处理"
date:   2018-03-11 16:36:21 +0100
categories: jekyll update
---

#### analyzer表示产生token的策略

* StandardTokenizerFactory 按标点和空格进行分割。但.之后不紧跟空格不进行分割，@不算为标点，所以邮箱地址会当做一个token
* PatternTokenizerFactory 按正则表达式进行分割(group=-1)或者提取(group不等于-1)
* KeywordTokenizerFactory 整个作为一个token，即没有进行分割


[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
