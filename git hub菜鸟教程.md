# 网站

|                                |                                                              |      |
| ------------------------------ | ------------------------------------------------------------ | ---- |
| git hub 网站                   | https://github.com/<br />用户名 lanchunhong<br />密码 l_8****9 |      |
| git 工具下载                   | git-scm.com                                                  |      |
| 怎么下载git                    | https://blog.csdn.net/qq_37512323/article/details/80693445   |      |
| git下载后怎么生成key           | git bash进入git操作界面<br />git config --global user.name lanchunhong<br />git config --global user.email "13521534675@163.com"<br />ssh-keygen -t rsa -C "13521534675@163.com"<br />输入git key文件名称，可以直接回车：Enter file in which to save the key (/c/Users/lanchunhong/.ssh/id_rsa): <br />输入密码：可以直接回车<br />文本编辑器打开就是key了：MyGitHubKey.pub |      |
| 我本地生成的key在哪里          | c:\Users\lanchunhong\.ssh\MyGitHubKey.pub                    |      |
| 生成key之后如何加到git hub网站 | https://blog.csdn.net/william_n/article/details/103280866?utm_medium=distribute.pc_relevant_t0.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-1.control&dist_request_id=&depth_1-utm_source=distribute.pc_relevant_t0.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-1.control<br />进入git config：https://github.com/settings/keys<br />New SSH key<br />MyGitHubKey.pub的内容复制后确认<br />本地测试key设置完成：ssh git@github.com<br />如果连不上的话，可以用这个命令调试：ssh -T -v git@github.com |      |
| 如何上传文件                   | https://github.com/lanchunhong/lanchunhong                   |      |
|                                | git init<br />git add README.md<br />git commit -m "first commit"<br />git branch -M master<br />git remote add origin https://github.com/lanchunhong/lanchunhong.git<br />git push -u origin master |      |

