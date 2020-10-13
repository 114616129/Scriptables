# Scriptables
iOS14桌面组件神器（Scriptable）原创框架，脚本开发教程、精美作品分享！    
本项目的框架和插件代码，都是本人手机上一个一个字符屏幕敲出来，一行一行代码调试的用心作品    
如果能得到您的喜欢，欢迎点个 ★ Star ★ 给予小支持，感谢您的使用，也同时欢迎大家一起参与改进完善 ❤️    

[国内 Gitee 仓库地址](https://gitee.com/im3x/Scriptables)    

👉 [点击查看 5 分钟演示视频](https://v.qq.com/txp/iframe/player.html?chid=17&vid=c31599njg4i&autoplay=true&full=true&show1080p=true)

![screenshot.jpg](https://i.loli.net/2020/10/13/hTVMr3EWO1xCNGL.jpg)

# 快速使用
1. iPhone 上下载 [Scriptable](https://apps.apple.com/cn/app/scriptable/id1405459188) App（确保你的系统已更新为 iOS14+）    
2. Safari点击下载：[国内Gitee源，推荐](https://im3x.cn/scriptables/Loader.Gitee.scriptable)、[GitHub版源](https://im3x.cn/scriptables/Loader.Github.scriptable)，然后点击下载的文件，用`Scriptable` App打开
2. 手动版：打开App，点击右上角 + 号，复制项目中对应的 [loader.github.js](loader.github.js) 或 [loader.gitee.js](loader.gitee.js) 代码    
3. 长按桌面，添加组件，选择 `Scriptable`，然后点击组件配置，选择刚刚保存的脚本，下方的参数格式为：`插件名@版本号:自定义参数`     
例如，我要显示`one`每日图文组件，配置下方输入`one`或`one@latest`即可（显示昨天的文章输入配置`one:1`，依此类推）。    

![](https://i.loli.net/2020/10/12/xf5utXvBWdC3F1g.jpg)

**更多插件的配置参数，请查阅插件目录的`README.md`说明**

# 组件列表
> 参数的意思，就是添加桌面组件时，选择加载器，然后下方参数中输入的内容    
> 更多参数配置，可以进入项目代码库中组件的目录，有更详细说明    

|名称|说明|示例参数|
|---|---|---|
|[one](one/)|韩寒ONE·一个图文|`one`|
|[v2ex](v2ex/)|V2EX 最新、最热文章|`v2ex@api`|
|[bing](bing/)|Bing 每日必应壁纸|`bing`|
|[zhihu](zhihu/)|知乎热榜等 |`zhihu`|
|[weibo](weibo/)|微博热搜榜|`weibo`|
|[一言](一言/)|随机更新一句话|`一言`|
|[毒鸡汤](毒鸡汤/)|随机更新一条毒鸡汤|`毒鸡汤`|
|[彩云天气](彩云天气/)|显示当前位置的天气预报情况|`彩云天气`|
|[彩票开奖](彩票开奖/)|展示最近一起开奖内容|`彩票开奖`|
|[知乎日报](知乎日报/)|显示知乎日报文章信息|`知乎日报`|
|[网易云音乐](网易云音乐/)|网易云音乐热评等|`网易云音乐@热评`|

## 框架优势
1. 简单方便，无需像其他组件一样，一个个复制代码编辑保存添加。框架直接添加一个加载器，后续全靠灵活的配置    
2. 灵活更新，插件有新功能，直接在线更新最新版本，而无需再手动复制代码保存等操作    
3. 功能强劲，经过多次的代码重构，解决了无数个坑的经验，保证了插件的更稳定运行环境    
4. 开发速度，直接套用模板，获取数据、展示数据，非常的简单， **插件代码还可以直接单独脱离框架执行**

## 插件开发
每一个项目，都创建一个文件夹，可以是中英文，最好不要有其他特殊符号。    
文件夹中存放该项目的版本号等文件，比如：    
1. `latest.js` 最新版本代码文件    
2. `README.md` 插件说明使用文档    
3. `v2.0.0.js` 其他版本或功能区分文件    

测试的时候，添加桌面组件，选择加载器，然后参数输入格式：`项目文件夹名@版本号:参数`，比如`v2ex`项目中有个`api.js`代码文件，传递：`v2ex@api:hot`类似格式的配置，也可以直接输入项目名即可（版本号默认latest，参数默认脚本定义）

插件代码，请直接复制项目中的`template.sample.js`模板编辑

## 教程系列
> 公众号集合文章：[#scriptable](https://mp.weixin.qq.com/mp/appmsgalbum?__biz=MzI5NTIwMDQxOA==&action=getalbum&album_id=1546917207903928321&scene=173#wechat_redirect)

1. [Scriptable 神器试玩，创建一个显示自定义标题内容的 iOS14桌面组件](https://mp.weixin.qq.com/s?__biz=MzI5NTIwMDQxOA==&mid=2247484293&idx=1&sn=128fd10f72e8bf0778d9e7575fa85c4a&chksm=ec567048db21f95eb223ad4504405de12612b94f5caa4c4cd611c448ee3b374a059d66c7acbe&scene=178#rd)
2. [Scriptable 神器实战2 —— 给桌面组件添加自定义背景图片](https://mp.weixin.qq.com/s?__biz=MzI5NTIwMDQxOA==&mid=2247484299&idx=1&sn=cddb9bc6af87eb8b63fb2b893e382111&chksm=ec567046db21f950b700d5845fe3778099c3888983ffd0a173f3f2dde7092bf3f862161add90&scene=178#rd)
3. [Scriptable 神器实战3 —— 夜间模式动态展示](https://mp.weixin.qq.com/s?__biz=MzI5NTIwMDQxOA==&mid=2247484312&idx=1&sn=967781d268224b794a21ddb940324f77&chksm=ec567055db21f943979e092ebb4195864590212393b1b8f7f5b3d4ea84f7fdf11eec7f56b48f&scene=178#rd)
4. [Scriptable 神器实战4 —— 获取桌面组件的大小以自动展示内容](https://mp.weixin.qq.com/s?__biz=MzI5NTIwMDQxOA==&mid=2247484324&idx=1&sn=b7bc2a4a513f719ce6e6423d03ba6803&chksm=ec567069db21f97ff3407d053aa708d408058c525d1cb9fc80a64ce9ca0e6b9133f4568a20e0&scene=178#rd)
5. [Scriptable 神器实战5 —— 给桌面组件添加一个渐变色背景](https://mp.weixin.qq.com/s?__biz=MzI5NTIwMDQxOA==&mid=2247484331&idx=1&sn=82802dd0d11fee43587f71cac6ce6109&chksm=ec567066db21f970ac13bf9ff902cee43475919a9e136a16eb2766c9cef5a6518b6d14bcab57&scene=178#rd)
6. [Scriptable神器实战6 —— 给背景图片加上半透明遮罩](https://mp.weixin.qq.com/s?__biz=MzI5NTIwMDQxOA==&mid=2247484345&idx=1&sn=7ebaa57bdf09ca5517b9ca58a12f88b8&chksm=ec567074db21f96234bd0591530b02c0c9bb3c951923fee19ebbb877e52aac56d5b8bd4d27af&scene=178#rd)
7. [Scriptable神器实战7 —— 获取用户添加组件时的自定义参数](https://mp.weixin.qq.com/s?__biz=MzI5NTIwMDQxOA==&mid=2247484350&idx=1&sn=f4c5b25b2d9f7e66bdfbe9150e234864&chksm=ec567073db21f965a5164e2ab27bacfc2b246e4be31ca3a4f23fb96e9c5d543e4ac97310b7bc&token=1302596105&lang=zh_CN#rd)
8. **[Scriptable 实战之 —— 桌面组件交互之王](https://mp.weixin.qq.com/s?__biz=MzI5NTIwMDQxOA==&mid=2247484386&idx=1&sn=c88ddafedad97a3bcfed50f92d16ac5a&chksm=ec56702fdb21f939a3b45305a7a9056fd25bbcb41b69d6f9c7ced34ff46f5f32a913d40ba1ae&scene=178#rd)**.   
9. [Scriptable神器实战 8 —— 本地存储 Keychain 用法](https://mp.weixin.qq.com/s?__biz=MzI5NTIwMDQxOA==&mid=2247484386&idx=2&sn=1b481bb66e0c373d8fd39dfede72575a&chksm=ec56702fdb21f939f07701aeead4375abc02450177565c96d937f9bfa0262ed12e378bca108a&scene=178#rd)

更多文章连载更新中，扫一扫关注【古人云】公众号，第一时间获取更新：    
![](https://i.loli.net/2020/10/13/9hXdRNUg5qSreHk.jpg)
