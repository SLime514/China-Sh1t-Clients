# China-Sh1t-Clients
此仓库会收录来自中国的构思我的手艺客户端
## 第一位:EdgeInjector 2k25 10/25最新最热FullSRC
### 它是什么东西?
它是由一个垃圾人基于未知的狗屎Base开发的布吉岛垃圾热注入,这个热注入的视觉十分的狗屎,都没有Myau美观
### 它是如何被破解的?
 - 在a/xn这个class中 我们发现了hwid计算逻辑与客户端初始化逻辑同时发现了http向服务器阻塞发送验证请求。
 - 请求的回复是一串数字 被转化为36进制的BigInteger。
 - 验证方法是对BigInteger进行模运算。如果数值不对就会触发绷端逻辑。
### 笑点解析
 - 关于暗装：在TickEvent中有0.01%的概率触发key（BigInteger）检查，同样是进行模运算。
 - 关于绷端：将Minecraft类中的随机字段设为null。
 - 关于起义搞笑aicode的Transfomer：可能是豆包只会使用javaasm coreapi吧反正很搞笑。
 - 关于ClassLoader逻辑：不知道为什么，edge的所有class都会被加载到一个独立的URLClassLoader中，大概是为了绕过盒子的class检测吧。
