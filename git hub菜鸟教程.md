# 工具提前准备

|                 |                                                            |      |
| --------------- | ---------------------------------------------------------- | ---- |
| chome语言设置   | 设置->高级->语言->英文                                     |      |
|                 |                                                            |      |
| git 工具下载    | git-scm.com                                                |      |
| 怎么下载git     | https://blog.csdn.net/qq_37512323/article/details/80693445 |      |
| 本地下载好的git | D:\LanchunhonNote\2 学习\1 工具\Git-2.31.1-64-bit.exe      |      |

# git hub网站

|              |                                                              |      |
| ------------ | ------------------------------------------------------------ | ---- |
| git hub 网站 | https://github.com/<br />用户名 lanchunhong<br />密码 l_8****9 |      |

# 下载好怎么用

| 首次进入要配置key              |                                                              |
| ------------------------------ | ------------------------------------------------------------ |
| git下载后怎么生成key           | git bash进入git操作界面<br />git config --global user.name lanchunhong<br />git config --global user.email "13521534675@163.com"<br />ssh-keygen -t rsa -C "13521534675@163.com"<br />输入git key文件名称，可以直接回车：Enter file in which to save the key (/c/Users/lanchunhong/.ssh/id_rsa): <br />输入密码：可以直接回车<br />文本编辑器打开就是key了：MyGitHubKey.pub |
| 我本地生成的key在哪里          | c:\Users\lanchunhong\.ssh\MyGitHubKey.pub                    |
| 生成key之后如何加到git hub网站 | https://blog.csdn.net/william_n/article/details/103280866?utm_medium=distribute.pc_relevant_t0.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-1.control&dist_request_id=&depth_1-utm_source=distribute.pc_relevant_t0.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-1.control<br />进入git config：https://github.com/settings/keys<br />New SSH key<br />MyGitHubKey.pub的内容复制后确认<br />本地测试key设置完成：ssh git@github.com<br />如果连不上的话，可以用这个命令调试：ssh -T -v git@github.com |
| **日常如何上传文件**           |                                                              |
| 项目地址如何获取               | github点击右上角用户，your responsitories                    |
|                                | https://blog.csdn.net/kuangsonghan/article/details/78970455<br />创建文件夹<br />git init<br />git clone https://github.com/lanchunhong/Home.git<br />git add xxx ==表示添加指定文件<br />git add . ==表示添加所有文件<br />git commit -m "你想写的注释"<br />git remote add origin https://github.com/lanchunhong/Home.git ==本地与远程关联<br />git pull origin master ==master或者其他分支名<br />git push -u origin master在这个步骤中可能会有弹窗要你输入你的用户名和密码，按照指示操作即可 |
| 项目列表                       | https://github.com/lanchunhong?tab=repositories              |
| 参考                           | https://github.com/lanchunhong/lanchunhong                   |
| 不存在                         | git init ==初始化一个git的本地仓库<br />git add “git hub菜鸟教程.md” ==添加本地文件，也可以用git add . 添加所有文件<br />git commit -m "first commit" ==提交到本地仓库 <br />git branch -M main  ==创建main分支<br />git remote add origin https://github.com/lanchunhong/Home.git  ==先将本地仓库与远端仓库建立一个链接，远端仓库名origin，远端仓库真实地址https://github.com/lanchunhong/Home.git<br />git push -u origin main == 把本地仓库main提交到远端仓库origin |
| 已存在                         | git add “git hub菜鸟教程.md” ==添加本地文件，也可以用git add . 添加所有文件<br />git commit -m "20210411" ==提交到本地仓库 <br />git remote add origin https://github.com/lanchunhong/Home.git ==先将本地仓库与远端仓库建立一个链接，远端仓库名origin，远端仓库真实地址https://github.com/lanchunhong/Home.git<br />git push -u origin main == 把本地仓库main提交到远端仓库origin |
| **不想要的工程如何删除**       |                                                              |
|                                | https://github.com/lanchunhong?tab=repositories<br />进入项目<br />进入setting<br />最底部**Delete this repository**<br />输入要求填写的黑体字<br />输入密码 |

# git其它命令

| 增                        |                                                              |      |
| ------------------------- | ------------------------------------------------------------ | ---- |
| 创建新分支                | git checkout -b xxx                                          |      |
|                           |                                                              |      |
| **删**                    |                                                              |      |
|                           |                                                              |      |
| **改**                    |                                                              |      |
| 切换分支                  | git checkout master                                          |      |
| 回退一个版本              | git reset --hard HEAD^<br />git reset --hard HEAD~1<br />git reset --hard HEAD~100<br />git reset --hard ID ==其中ID为git log查询到的commit版本号 |      |
|                           |                                                              |      |
| **查**                    |                                                              |      |
| 查本地分支                | git branch                                                   |      |
| 查远端分支                | git branch -a                                                |      |
|                           | git reflog                                                   |      |
| 查当前git下载的是哪个分支 | git status                                                   |      |

# git说明

| 介绍    | https://pypypy.blog.csdn.net/article/details/104551896?utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-2.control&dist_request_id=&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-2.control |      |
| ------- | ------------------------------------------------------------ | ---- |
| 来源    | 因为没有商用软件，Linus花了两周时间自己用C写了一个分布式版本控制系统 |      |
| 2大特点 | 版本控制：可以解决多人同时开发的代码问题，也可以解决找回历史代码的问题。<br /><br />分布式：Git是分布式版本控制系统，同一个Git仓库，可以分布到不同的机器上。首先找一台电脑充当服务器的角色，每天24小时开机，其他每个人都从这个“服务器“仓库克隆一份到自己的电脑上，并且各自把各自的提交推送到服务器仓库里，也从服务器仓库中拉取别人的提交。可以自已搭建这台服务器，也可以使用GitHub网站。 |      |
|         | 工作区------git add------暂存区------git commit------本地仓库/本地分支/master------git push------远程仓库 |      |
|         |                                                              |      |

