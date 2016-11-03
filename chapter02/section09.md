# 公众号接口

## 1. 公众号消息会话

目前公众号内主要有这样几类消息服务的类型，分别用于不同的场景。

#### 群发消息

公众号可以以一定频次（订阅号为每天1次，服务号为每月4次），向用户群发消息，包括文字消息、图文消息、图片、视频、语音等。

#### 被动回复消息

在用户给公众号发消息后，微信服务器会将消息发到开发者预先在开发者中心设置的服务器地址（开发者需要进行消息真实性验证），公众号可以在5秒内做出回复，可以回复一个消息，也可以回复命令告诉微信服务器这条消息暂不回复。被动回复消息可以设置加密（在公众平台官网的开发者中心处设置，设置后，按照消息加解密文档来进行处理。其他3种消息的调用因为是API调用而不是对请求的返回，所以不需要加解密）。

#### 客服消息

在用户给公众号发消息后的48小时内，公众号可以给用户发送不限数量的消息，主要用于客服场景。用户的行为会触发事件推送，某些事件推送是支持公众号据此发送客服消息的，详见微信推送消息与事件说明文档。

#### 模板消息

在需要对用户发送服务通知（如刷卡提醒、服务预约成功通知等）时，公众号可以用特定内容模板，主动向用户发送消息。

## 2. 公众号内网页 

对于公众号内网页，提供以下场景接口：

#### 网页授权获取用户基本信息

通过该接口，可以获取用户的基本信息

#### 微信JS-SDK

是开发者在网页上通过JavaScript代码使用微信原生功能的工具包，开发者可以使用它在网页上录制和播放微信语音、监听微信分享、上传手机本地图片、拍照等许多能力。

## 3. 微信开发者文档

[**微信开发者文档网址 https://mp.weixin.qq.com/wiki/home/index.html**](https://mp.weixin.qq.com/wiki/home/index.html)

![微信开发者文档](/images/wechat_dev_doc.png)