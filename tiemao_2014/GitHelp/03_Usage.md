TortoiseGit基本操作
==

## 3. <a name="tgitoperate">TortoiseGit使用与操作</a>

使用 Git命令有时候确实不怎么方便,特别是每次都要输入密码,如果配置 SSH 的方式,又实在是很麻烦.(当然,必须使用 Windows 神器才有方便友好的客户端图形界面啦!!!)

关于 TortoiseGit 的安装请参考 [前一小节](02_TortoiseGit.md).

### 3.1 克隆项目

打开资源管理器(我的电脑/计算机), 进入规划好的某个目录中, 然后在空白处点击鼠标右键, 选择 TortoiseGit --> 克隆... (Clone...). 

![](401_rightclick.png)

弹出克隆项目对话框:

![](402_tgitclone.png)

在对话框的 URL中输入项目地址,如: 

	https://github.com/cncounter/LispGentleIntro.git

确定本地目录,然后点击 **确定** 按钮. 等待完成后,点击关闭按钮即可.


![](403_tgitcloned.png)


### 3.2 修改提交项目

项目克隆完成后(可以将克隆 clone 理解为 下载, 检出 checkout 操作). 修改本地项目中的某些文件,如 将 `README.md` 修改为如下内容: 

	LispGentleIntro
	===============
	
	Lisp-符号计算入门指引翻译
	
	<a href="http://cncounter.duapp.com/">天朝计数器</a>

还可以试试增加一些文件. 如 `files.txt` .

然后在本地项目的空白处点击鼠标右键, 选择 **TortoiseGit --> 提交(C) -> "master"...**  或: Commit -> "master".... 

![](404_rcick_commit.png)

弹出提交（Commit）对话框:

![](405_commitlog.png)

作为好习惯,填写提交日志,勾选需要提交的文件,然后点击 "确定" 按钮, 即提交到本地仓库.

![](406_commit2push.png)



### 3.3 将提交到本地的项目推送到在线仓库

推送是提交的下一步操作. 

在本地项目的空白处点击鼠标右键, 选择 **TortoiseGit --> 推送...**  或: Push.... 

![](407_tgit_rclick_push.png)

弹出推送(push)对话框:

![](408_tgit_push.png)

一般保持默认,点击 “**确定**” 按钮. 

然后弹出推送进度界面, 可能要求你输入用户名:

![](409_username.png)

确定OK，然后要求输入密码:

![](410_pass.png)

密码输入正确后,OK，显示推送成功界面:

![](411_pushok.png)

如果你按照上一小节的设置操作,则输入密码以后会记住密码. 密码会明文保存在 `C:\Users\Administrator\.git-credentials` 这种文件中, 请小心使用.


### 3.4 拉取项目(pull ...)

如果本地的项目没有在线仓库的新,则需要执行拉取操作(Pull ...).

在本地项目的空白处点击鼠标右键, 选择 **TortoiseGit --> 拉取...**  或: Pull.... 

![](412_rck_pull.png)


弹出拉取(pull)对话框:

![](413_pull_dialog.png)

【如果拉取有BUG,请不要使用 rebase, 下载[最新的 TortoiseGit](http://download.csdn.net/detail/renfufei/9738152) 即可】, 进入 拉取进度界面:

![](414_pulled.png)

<del>然后执行变基:</del>

【如果拉取有BUG,请不要使用 rebase, 下载[最新的 TortoiseGit](http://download.csdn.net/detail/renfufei/9738152) 即可】

![](414_c_base.png)

然后完成即可.

这应该是 TortoiseGit 的一个BUG, 要解决这个问题,请参考 [解决 TortoiseGit 诡异的 Bad file number 问题](05_BadFileNumber.md) (或者可以换回老版本. 如果你没有出这个问题,那么,可能是我的机器哪里损坏了).


## 4. 更复杂的操作

当然,多人协作过程中,避免不了会有各种意外情况需要处理,比如冲突,合并,变基等等, 关于这些复杂的操作,请参考: [GotGitHub系列: http://www.worldhello.net/gotgithub/01-explore-github/010-what-is-github.html](http://www.worldhello.net/gotgithub/01-explore-github/010-what-is-github.html)



## 5. 相关文章

1. [目录](GitHelp.md)
1. [安装及配置Git](01_GitInstall.md)
1. [安装及配置 TortoiseGit](02_TortoiseGit.md)
1. [基本使用方法](03_Usage.md)
1. [MarkDown示例](04_MarkDownDemo.md)
1. [解决 TortoiseGit 诡异的 Bad file number 问题](05_BadFileNumber.md)
1. [加入QQ群GitHub家园: 225932282](http://jq.qq.com/?_wv=1027&k=WHbwkD)



日期: 2014-11-27

作者: [铁锚: http://blog.csdn.net/renfufei](http://blog.csdn.net/renfufei)
