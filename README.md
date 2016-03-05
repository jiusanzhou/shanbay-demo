# Shanbay Demo

您好，您之所以能看到这个页面，是因为，

1. 您点击了右上角的“关于”；
2. 您还没有登陆。

如果是 2 的话，而且您正愿意体验功能，恰好，您之前有注册过，请点击登陆链接，
如果您这是第一次使用，劳烦您点我注册。
这是我为了应聘扇贝的开发职位，所做的测试题，下面是原邮件内容：
> 你好！我是扇贝网的工程师。非常高兴你选择应聘扇贝网。 我这里有一个小作业，以便我们后面面试环节更好的沟通。 
假设你现在想做一个简单的背单词应用，具体提供下面的5项功能：
* 1. 用户可以根据自己的英语水平，例如 四级，六级，雅思，和托福 来设置自己背单词的范围；
* 2. 每个用户可以设置每天背多少单词
* 3. 用户背单词过程中能够添加笔记， 也可以查看其他用户共享的笔记
* 4. 用户背单词过程中，可以看到单词，单词的解释和例句。
* 5. 背单词的时候还可以看到近义词，请考虑提供这个单词的两个近义词（如果有的话）
我们要求作业用 Python, 最好是 基于 Django 框架来完成， Web 页面可以基于 bootstrap 来简化你的开发流程。 
我们希望你最迟在收到邮件的 2 周内能提交给我们代码，但如果你能在 1 周之内完成会有额外加分。 
如果你需要额外延长你的时间，请务必提前和我们联系。
我们会非常认真得阅读你的代码， 在后续的沟通中我们将基于你的代码来讨论， 如果你在开发过程中有什么问题，可以和我们沟通。


首先我很感谢扇贝网给我这次机会，当然这不是冠冕堂皇的陈词滥调，是真诚的感谢！
扇贝在英语应用领域贵为翘楚，实乃行业的标杆，无不动恻隐加盟之心。
所以我很重视这个机会，实说，我于26日上午收到邮件，定三日之期欲完成之。
并非欲速则不达，事不与人愿耳！

由于我没有电脑，只能使用原公司的电脑来完成开发，白天公司里面需要，我只能是晚上到公司来使用。
幸亏在离职前，使用的正是现在这台，所以前端的开发环境就无需重新搭建。
实际开始是28日起，这一天主要是完成了“架构”和数据表的设计工作以及环境搭建。
29日至2号因朋友被骗3万余元，到上海去耽误了3天（未果）！
逾期！

这里便是连续几个夜晚的工作成果。

### 目标

* 前后端分离单页应用

### 技术“架构”
* Django作为API提供服务器
* 前端使用Vue.js开发

其中，Django使用REST framework来简化RESTful接口的开发。

### 预期的功能

* 单词数据本地存储减少数据请求
* 邮箱注册并激活，第三方帐号登陆
* 错词统计，学习记录
* 继续明日任务
* 生词本
* 造句，笔记发表与分享
* 造句，笔记点赞评论
* 个人学习记录，造句，评论，笔记管理
* 广场平台，群聊
* 后台管理
> 邮件说明了需要提供，近义词功能，若不取用别的现有数据，我这里已经能够做到不完全正确的近义词获取。
单词的释义都进行了最小化，此时只需要计算单词相关性即可。
剩下的一些功能均为API的实现和数据的操控，基本架构已经实现。

### 截三月六日0:57时已经完成的功能

* 背单词
* 注册，登陆
* 信息修改
* 单词数据本地存储减少数据请求
* 例句笔记获取
* 部署
* 已知BUG
* 待改进部分

### UI

* 随机获取单词
* 导航条内容不能随而登陆更新，使用了location.reload()
* 点击关于，无法加载内容，布局出错，使用了location.reload()
* 信息修改GET请求

### 后记

写到这里，才意识到我是应聘后端开发，起码这次测试应该花更多的时间在Django的编码上。
但，截止目前我在前端和后台所花的事件大体相当，而且前端的时间很大一部分还是在美化布局，美化颜色，美化字体......
或许这就是所谓的完美主义与理想主义，哪怕是和泥巴也要和成圆的！


全文完
周辉，于合肥国家大学科技园
二〇一六年三月六日深夜


### Building

``` bash
npm install
# watch:
npm run dev
# build:
npm run build
```
