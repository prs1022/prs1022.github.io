---
title: chatgpt
date: 2023-06-01 16:43:31
tags:
- gpt
- AIGC
categories: 
- AI
---

# chatgpt


- web地址: https://chat.openai.com/ 需要科学上网，早期可以注册，现在不行了
- flowgpt: 现在科学上网可以注册，免费，每天登陆可以claim 25 积分，每次chat消耗积分
- [AIhunt导航](https://www.aihunt.one) 是一个不错的导航站， 里面有很多资源
- [在线小工具](http://tools.jb51.net/)
- [有趣的网站](https://lks.cc/)



## prompt
在用gpt的时候，prompt提示词很关键，上面的flowgpt就是专门为提示词做的一个社区项目，创始人就是想把大家的idea集中起来，做各种各样的template，大家互相分享交流学习。

还有这样的网站[Awesome提示词](https://prompts.chat/)，里面有个很有意思的prompt，
**Act as a Python interpreter**
```
I want you to act like a Python interpreter. I will give you Python code, and you will execute it. Do not provide any explanations. Do not respond with anything except the output of the code. The first code is: “print(‘hello world!’)”
```

接下来输入给gpt的就是各种各样的python代码，gpt会给出相应的输出结果，我试了一下结果很正确，然后让它切换到java编译器，在网上找了一些枯燥晦涩的java笔试题喂给他， 他第一道居然就答错了。 anyway， 在我们告诉他 **you are wrong**后，很快啊，它又generate了一段回复，这回它对了。

尽管它有时候第一次不能完美回答，但是它的出现给了我们很多idea，以前从未有过的， 就拿这层出不穷的prompt来说，确实集思广益了。有句话拿出来跟大家分享，**有时候会问问题比知道答案更重要**， 在gpt身上体现的淋漓尽致， 有时候不是它回答的不是我们想要的，而是我们问的不够好 不够完善。


## template

我在flowgpt中建立了两个flow，可以看作就是模板吧。

我当时的需求是想用gpt给我生成一些语料 corpus

在NLP算法开发之前有大量的时间是需要标注语料的，当然有专门的digital marker来做这件事。也有一些工具可以做，但是最好的还是人工标注，以应对复杂的语言环境，反问啊，疑问啊，还有一些摸棱两可的句子，总之很复杂就是了。 但是简短的一些语义的泛化其实就有迹可循了。

例如我们要问 **明天上海的天气怎么样?**

一般的泛化说法就是 
1. 加前缀助词 帮我看看....
2. 加尾缀词 ...你知道吗
3. 同义词的替换 明天换成明日，上海换成魔都等等
4. 语句的倒装，天气怎么样在明天的上海。。这个例子可能不是特别好。。。。 
5. 中间加上一些词，不重要的。说不重要指的是不是实体词，或者准确点说是天气这个垂域不需要关心的实体词。


ok， 以上是我能想到的一些泛化说法了， 至于还有其他的让我来问gpt吧，因为规则都是人事先想好的，就像正则一样，只能产生规则内的一些说法，超出规则外的一些是我人脑短时间难以考虑到的。


ok，看看我在flowgpt建立的模板吧

``` text
我给你一个语料标注模版，例如，“请给我查一下上海下周一到下周三的天气”，标注结果为“请给我查一下[上海](poi)[下周一到下周三](time)的天气”。现在我给你一批语料，帮我按照这个规则去生成标注后的结果。
```
这里给出的一个模板就是我上面陈述的，但是又不止于天气，其实我可以问导航、电话、系统设置等方面的句子。
这里的标注只限于实体词的抽取了，NLU还有一步是要区分这个句子的意图 intent，也就是个分类模型， 这个也可以用gpt帮忙去做。


## Learn English

有时候需要找一个人练习英语，口语的条件有点难得，但是文字的回复我们可以有啊，跟gpt学英语是再好不过的了。


ok， 就更新到这里吧，以后想起来继续写。

>> 这个博客昨天刚知道怎么搭建，以前接触过wordpress，还有一个docsify ,感觉还是这个好用啊，哈哈哈。markdown用的还不太熟练，文本不够丰富，我觉得有必要多练习，以后就用这个记录学习，感悟点滴了。