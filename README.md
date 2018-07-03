# web-rtmp-streamer

本项目使用js+swf实现了一个rtmp推流器。有效兼容腾讯云等标准rtmp推流服务。可以直接[访问DEMO](https://lujunda.github.io/web-rtmp-streamer/)查看效果。

本项目是在**网易云推流DEMO**基础上进行了二次开发，与原版相比，有以下改进：
* 去除了原版只能向网易云推流的限制
* 解决了原版无法兼容新版chrome的问题（"Cross-origin plugin content from  must have a visible size larger than 400 x 300 pixels, or it will be blocked. Invisible content is always blocked."）
* 解决了原版使用JSON.parse()前没判断类型导致推流失败的bug
* 剥离原版各种http请求（如心跳接口、获取网易云cdn地址等），实现纯净无监控推流器。
