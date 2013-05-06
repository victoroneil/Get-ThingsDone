<a target="_blank" href="http://wp.qq.com/wpa/qunwpa?idkey=554811f77edb8de205df4340567b4a74e421808b0a847a2a633b801c37774a08"><img border="0" src="http://pub.idqqimg.com/wpa/images/group.png" alt="中国PowerShell资源交流" title="中国PowerShell资源交流"></a>
# Get-ThingsDone
**最新版本：1.0.4.1，发布时间：2013-04-16**

![logo](https://raw.github.com/victorwoo/Get-ThingsDone/master/gtd_logo.png)

# 欢迎使用
这是一个基于GTD思想和PowerShell技术的文件管理脚本，能够将您从繁杂的待处理文件中解脱出来。

**请注意，本程序并不能“自动”帮您进行日常工作。本程序只是提供了一种操作规范和进行一些辅助处理工作。**

# GTD简介
> GTD是英文Getting Things Done的缩写，是一种行为管理的方法，也是David Allen写的一本书的书名。
> GTD的主要原则在于一个人需要通过记录的方式把头脑中的各种任务移出来。通过这样的方式，头脑可以不用塞满各种需要完成的事情，而集中精力在正在完成的事情。

# 使用环境
- Windows XP/2003/Vista/2008/2008R2/8/2012
- PowerShell 2.0/3.0

# 功能特色
- 严格遵循GTD思想。
- 遇到重名的文件会自动更名，不会丢失任何文件。

# 快速使用方法
- 将压缩包解压缩到硬盘上的固定文件夹，例如`D:\GTD`。
- 运行`GTD.cmd`。
- 将文件分类存放至相应文件夹。
- 下次运行`GTD.cmd`时，将按GTD的思想整理文件。

# 详细使用说明
## 目录结构
- `0.STUFF` - `收集箱`，用于收集零碎的材料（指文件/文件夹），准备好做下一步的处理。
- `1.TODAY` - `今日待办`，用于存放今日待办的材料。
- `2.TOMORROW` - `明日待办`，用于存放明日待办的材料。
- `3.UPCOMING` - `下一步行动`，用于存放紧接着要处理的材料。对于每个需要你关注的事项，定好什么是你可以实际采取的下一步行动。例如，如果事项为“写项目报告”，下一步行动可能会是“给Fred发邮件开个简短会议”，或者“给Jim打电话问报告的要求”，或者类似的事情。虽然要完成这个事项，可能会有很多的步骤和行动，但是其中一定会有你需要首先去做的事情，这样的文件就应该存放在“下一步行动”文件夹中。
- `4.CALENDAR` - `日程`，用于存放确定某个日期需要处理的材料。当到达指定日期前一天时，其中的材料将会自动移动到`2.TOMORROW` - `明日待办`文件夹中。请在在日程目录下，以“YYYY.MM.DD”形式，创建文件夹，以便脚本识别。
- `5.SOMEDAY` - `将来也许`，用于存放较长时期以后才需要用到的材料。这些材料你需要在某个点去处理，但是不是马上。
- `6.ARCHIVE` - `存档`，存放已处理好，舍不得删除的材料，用于将来备查。脚本将自动按“YYYY.MM”格式创建文件夹。

## 使用流程
- 将压缩包解压缩到硬盘上的固定文件夹，例如`D:\GTD`。
- 首次运行`GTD.cmd`，脚本询问您是否需要在用户登录时自动运行。
	- 如果您选择“否”，将不再提示。
	- 如果您选择了“是”，但日后不希望自动运行，请执行`uninstall.cmd`。
- 首次运行脚本之后，在您的目录之下将生成`0.STUFF`、`1.TODAY`等标准文件夹。请不要任意修改目录结构或在这些目录之外存放材料。
- 将日常工作材料放在相应的目录中。
- 每日开始工作前，运行一次脚本。
- 每日按照GTD的流程，逐项处理`0.STUFF`、`1.TODAY`、`3.UPCOMING`等文件夹中材料。
**请注意，本程序并不能“自动”帮您进行日常工作。本程序只是提供了一种操作规范和进行一些辅助处理工作。**

# 计划中的功能
- 制作成在线更新版本。
- 重构代码，添加注释。
- 做成多语言版。

## 2013-04-16
- 修正存档功能中不会移动文件的bug。
- 发布1.0.4.1版本。请更新到此版本以避免bug。

## 2013-04-11
- 修正存档功能中不会移动文件的bug。
- 发布1.0.4.1版本。请更新到此版本以避免bug。

## 2013-04-11
- 自动删除重复的文件。
- 将存档目录下游离的文件按日期归类。
- 发布1.0.4版本。

## 2013-03-19
- 排除GoodSync缓存文件夹。
- 更改自述文件，以便github自动显示。
- 发布1.0版本。

## 2013-03-15
- 撰写本文档

## 2013-03-14
- 添加Calendar功能
- 添加自动运行功能

## 2013-03-07
- 初始版本，实现了GTD的`收集箱`、`今日待办`、`明日待办`、`下一步行动`、`将来也许`功能。

# 参考材料
不了解GTD的同学请参考以下材料：

- [维基百科关于GTD的介绍](维基百科关于GTD的介绍 "http://zh.wikipedia.org/wiki/GTD")
- [百度百科关于GTD的介绍](百度百科关于GTD的介绍 "http://baike.baidu.com/view/406078.htm")
- [《搞定》](http://book.douban.com/subject/4849382/)（中文版）
- [《Get Things Done》](http://book.douban.com/subject/1849836/)（英文版）

# 引用版权声明
GTD® and Getting Things Done® are registered trademarks of [David Allen & Co](http://www.davidco.com/about-gtd "about gtd").
