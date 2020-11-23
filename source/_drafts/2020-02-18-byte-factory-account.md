---
title: 谈一谈关于账号密码的存储工具 | 账号箱
date: 2020-04-14
tags: [字节加工厂,账号密码]
---

账号箱，这个名字起得不太好，但是，又没有想到特别好的。账号密码这么敏感的信息，谁会想要保存在你这里，即使你说是离线保存在本地，那又怎样，谁知道是不是离线保存在本地？

所以，「账号箱」这个小工具，应该注定只有我一个用户，当然，它本身就是为了我自己而做的。

在那个还不是用手机号注册账号的年代，用户名真的是五花八门，有使用用户名的，有使用邮箱的，有的网站用户名不允许有下划线，有的不允许超过多少字符。逼得用户看到自己的起的用户名，都不知道是谁了。

相对而言，密码倒还没有那么复杂，因为大多数人为了避免麻烦，应该都使用的是同一套密码，稍微机灵点的，可能会分为高，中，低，三个档位的密码，用在不同类型的网站。再有点安全意识的，就会基于一个规则，给每个网站设置不同的密码，例如：固定字符+变量，admin123+58 是 58 的密码，admin123+qq 是 QQ 的密码。

我属于那种稍微机灵点，外加有点安全意识的那一类，通过这两种方式，记住常用的账号密码，倒问题不大。可是，时间一长，对于不常用的，脑子就不好使了。

这其实是痛点需求啊，于是，针对这个需求的应用也就诞生了，最有名的莫过于 1Password，它提供的功能很全，甚至于云端存储，密码自动生成，还内置了浏览器。但是，本质上，它就是一个密码箱。

我一直没有领会到这个软件的精髓，也无法理解为什么这么多人推荐使用它。特别是在苹果官方已经提供钥匙链功能，以及 Google 浏览器本身带有账号保存功能的前提下。在我看来，它就是一个键值对数据保存功能的记事本而已。

更是没法理解它的云端功能，我们已经在互联网上几近裸奔了，还要再多向一个第三方的公司交出我们的账号密码，想想也是不可思议。

在我看来，这种信息最好是记在自己的脑子里，脑子记不住，找个记事本记下就可以了，越是本地储存，越安全，不要过于相信任何的云服务，即使有时候确实很方便。

另外，记下来的也最好是经过加工的，而不是直接写上密码。能起到提醒的作用就可以了。

有点扯远了，回到需求本身，就是要一个能保存「键值对」信息的工具，一定是本地存储。

于是，我就做了这个小工具，只保存在微信本地缓存，换个手机登陆微信，数据是不会同步过去的，就是一个离线的简易记事本。除了账号密码信息的记录，凡是「键值」储存的数据 ，都可以方便的记录，例如，家人的身份证号等



如上图，是我的微信公众账号记录，早些时候注册太多，都记不清，哪个邮箱对应哪个账号了。

大致说完了，它的实现就不值一提了，基本没有用到什么新特性，仅仅只是表单的存储而已。