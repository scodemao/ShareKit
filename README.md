[![License MIT](https://img.shields.io/badge/license-MIT-green.svg?style=flat)](https://raw.githubusercontent.com/ibireme/YYText/master/LICENSE)&nbsp;

# ShareKit
This is a 3rd platform share helper.

Easily used and integrated.

Update 
3rd Platform Support:
SinaWeibo 
Tencent QQ
Tencent QQZone
Tencent WeChat

## Usage

```java
//Weibo

ShareTool.getSinaWeiboShareApi(Activity, AppConfig.WEIBO_APP_ID)
    .shareSinaWeibo(SinaWeiboParams, SinaWeibo.TYPE_WEBPAGE, new BaseIUListener()) ;

//QQ

ShareTool.getQQShareApi(Activity, AppConfig.QQ_APP_ID,"AppName")
    .shareQQ(QQParams, QQ.TYPE_IMAGE_TEXT,new BaseIUListener());

//WeChat TimeLine

ShareTool.getWeChatShareApi(activity, AppConfig.WX_APP_ID)
    .shareWeChatTimeline(WeChatParams, WeChat.TYPE_WEB_PAGE);

//WeChat Favourite

ShareTool.getWeChatShareApi(activity, AppConfig.WX_APP_ID)
    .shareWeChatFavourite(WeChatParams, WeChat.TYPE_WEB_PAGE);

//WeChat Friend

ShareTool.getWeChatShareApi(activity, AppConfig.WX_APP_ID)
    .shareWeChatSession(WeChatParams, WeChat.TYPE_WEB_PAGE);
```
## Dependence:

```java
compile 'com.squareup.picasso:picasso:2.3.4'

```
