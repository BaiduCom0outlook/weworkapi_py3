主要是企业微信发送消息以及回调，因为官方给的是python2的版本，而且因为给的代码库和范例是18年的，所有很多地方也有些坑，比如加密函数的过程中5个参数位置错位了之类的问题。
在官方给出的代码的基础上进行了更改，实现对企业微信消息发送以及回调的功能
官方地址https://github.com/sbzhu/weworkapi_python
主要更改callback文件夹中的WXBizMsgCrypt.py文件，迁移使用时将本项目中的替换即可
## callback/weixin.py
可用于回调验证。把用户在企业微信上对应的应用回复的内容记录在本地文件中。
## callback/sent_weixin.py
只接受经过校验的post数据包，并推送到企业微信上的指定应用
