# DanmakuChi-Server-Node
弹幕姬服务器端 Node (node.js) 版本

![微信号示例](https://raw.githubusercontent.com/wspl/DanmakuChi-Server-Node/master/attachments/wechat.png)

## 介绍
　　弹幕姬是一款「微信x桌面」弹幕系统，开发者可以通过轻松的绑定，在微信公众号与桌面弹幕之间建立交互关系。任何人都可以通过微信公众号创建自己专属的弹幕频道，任何用户都可以通过微信向客户端发送弹幕。

　　其中，服务器端（Server End）负责微信的交互，以及微信与客户端的中转对接。通常的，服务端需要一台开放 80 端口的公网服务器来运行。目前已经开发了 [Node 版本](https://github.com/wspl/DanmakuChi-Server-Node)。

　　客户端（Client End）负责与服务端的交互，进行弹幕的展示。目前已经开发了 [C# 版本](https://github.com/wspl/DanmakuChi-Client-CSharp)。

## 使用帮助

#### 生成频道二维码
推荐使用[草料二维码生成器](http://cli.im/)来生成频道二维码。

二维码文本格式：

`http://weixin.qq.com/r/<qrcodeToken>?dmk_channel=<channel>`

例如，「上师大弹幕姬」微信号中有个频道叫做 `Demo`，则二维码文本为：

`http://weixin.qq.com/r/MjoCGobEsdvOrcJ5928g?dmk_channel=Demo`

同时，这个二维码同样可以用于关注微信号。

## 技术栈
该 Node 版本的服务端中，涉及到的技术栈如下：
* ECMAScript 7
* [Node 4.2.1](https://nodejs.org/en/)
* [Express 4](https://github.com/strongloop/express)
* [Babel](https://github.com/babel/babel)
* [Socket.IO](https://github.com/socketio/socket.io)

## TODO List
- [x] 模块化 wechat.js

## Contributor
* [Plutonist(wspl)](https://github.com/wspl)

## License
GNU GPL V3