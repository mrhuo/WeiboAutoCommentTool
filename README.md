# WeiboAutoCommentTool

微博自动评论工具。
*警告：谨慎使用，仅供学习，不要做违法乱纪的事情。*

## 使用方法

* 登录微博
* 切换到发现页面 [https://d.weibo.com](https://d.weibo.com)
* F12打开浏览器控制台，把脚本内容全部复制粘贴到控制台，按回车
* 然后执行以下代码：

```
weiboAutoCommentTool.start({
  //评论内容，不填默认当前时间
  content: "哇，不错不错，很赞！"	,
  //评论间隔时间，默认秒
  delay: 10 * 1000 
});
```
## 其他工具
```
//停止自动评论
weiboAutoCommentTool.stop()
```

```
//查看评论统计
weiboAutoCommentTool.stat()
```
## 效果截图
![效果图](screen-shot.jpg)

## 测试日志（下列记录来自控制台复制）
```
weiboAutoCommentTool.start({
    content: '哇，真不可思议~~'
});

2018-05-07 13:08:48: WeiboAutoCommentTool start running...
2018-05-07 13:08:48: Use option: {"delay":10000,"content":"哇，真不可思议~~"}
2018-05-07 13:08:48: WeiboAutoCommentTool running now.
2018-05-07 13:08:48: Comment thread started.
----------------------------------------->
2018-05-07 13:08:48: Commenting 4236962166085444
2018-05-07 13:08:48: Comment list is not loaded, start loading...
2018-05-07 13:08:48: Waiting comment list loading...
2018-05-07 13:08:51: Sending comment content completed.
<-----------------------------------------
----------------------------------------->
2018-05-07 13:08:58: Commenting 4236975416123726
2018-05-07 13:08:58: Comment list is not loaded, start loading...
2018-05-07 13:08:58: Waiting comment list loading...
2018-05-07 13:09:01: Sending comment content completed.
<-----------------------------------------
----------------------------------------->
2018-05-07 13:09:08: Commenting 4236986120511160
2018-05-07 13:09:08: Comment list is not loaded, start loading...
2018-05-07 13:09:08: Waiting comment list loading...
2018-05-07 13:09:11: Sending comment content completed.
<-----------------------------------------

weiboAutoCommentTool.stat();
2018-05-07 13:09:13: Comment queue: 
["4236648663107765", "4236692271631492", "4236733615086129", "4236813700804304", "4236618468476778", "4236037263784663", "4235992158606659", "4236962166085444", "4236975416123726"]
2018-05-07 13:09:13: Commented list: 
["4236962166085444", "4236975416123726", "4236986120511160"]
2018-05-07 13:09:13: STAT: Pending comment 9, Total commented 3

----------------------------------------->
2018-05-07 13:09:18: Commenting 4236648663107765
2018-05-07 13:09:18: Comment list is not loaded, start loading...
2018-05-07 13:09:18: Waiting comment list loading...
2018-05-07 13:09:21: Sending comment content completed.
<-----------------------------------------

weiboAutoCommentTool.stop();
2018-05-07 13:09:21: User stoped
2018-05-07 13:09:28: Comment action stoped, exit.
2018-05-07 13:09:28: Comment thread action stoped, exit.
```
