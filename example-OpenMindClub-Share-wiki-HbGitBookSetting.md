# 配置 GitBook 简易指南

本指南适用于开智学堂的课程学员，用 GitBook 发布写在 GitHub 仓库里的笔记和作业。

用 GitBook 发布之前，你需要：

-  已注册 GitHub 账号，熟悉 GitHub 的基本操作（比如修订 GitHub 仓库文件内容并同步）。
-  已进入你所参加课程的 GitHub 仓库。

完成上述两步后，一般来说你只需要不到 5 分钟，就能把 GitHub 的内容已 GitBook 的形式发布，快来看下如何配置：

- [为什么要用 GitBook？](https://github.com/OpenMindClub/Share/wiki/HbGitBookSetting#%E4%B8%BA%E4%BB%80%E4%B9%88%E8%A6%81%E7%94%A8-gitbook%EF%BC%9F)
- [GitBook 简单配置教程](https://github.com/OpenMindClub/Share/wiki/HbGitBookSetting#gitbook-%E7%AE%80%E5%8D%95%E9%85%8D%E7%BD%AE%E6%95%99%E7%A8%8B)
- [给 GitBook 添加评论功能](https://github.com/OpenMindClub/Share/wiki/HbGitBookSetting#%E7%BB%99-gitbook-%E6%B7%BB%E5%8A%A0%E8%AF%84%E8%AE%BA%E5%8A%9F%E8%83%BD)
- [更多内容](https://github.com/OpenMindClub/Share/wiki/HbGitBookSetting#%E6%9B%B4%E5%A4%9A%E5%86%85%E5%AE%B9)
- [CHANGELOG](https://github.com/OpenMindClub/Share/wiki/HbGitBookSetting#changelog)

## 为什么要用 GitBook？

用作品说话，是开智学堂元范儿。学习不只是刷卡片、看视频、读文章，输出你的作品，用文字记录你的经验和感悟，教三个月前的自己学这门技能，「用输出倒逼输入」是更好的学习方法。

GitBook 是呈现你作品的好工具。你可用 Markdown 来编排内容，借助 Git 追踪记录你的改动，稍加配置，就能自动发布到 GitBook 上，形成界面漂亮的电子书。快来动手写一本关于本次课程的小书吧！

## GitBook 简单配置教程

以开智学堂「认知写作学」课程为例，为大家演示如何把 GitHub 仓库的内容以 GitBook 的方式发布。 网络好的话，5 分钟不到你就能配置好。

### 第一步：Fork 课程仓库

进入课程主仓库中，点击右上角的 Fork，选择自己的头像，添加到个人仓库中。这一步的作用，相当于把课程组做好的书目纲要复制到自己的仓库中，你只需填充内容就好。

![img](https://camo.githubusercontent.com/a844374a8ab3c4897833176a638c03503d1f5e3d/687474703a2f2f69342e7069696d672e636f6d2f3536373537312f356431323862626239363331386434372e706e67)
![img](https://camo.githubusercontent.com/dc392a0c0010f9d919132cd69818bd28b35bdf21/687474703a2f2f69342e7069696d672e636f6d2f3536373537312f326630663333626233366330643961392e706e67)

### 第二步：登陆 GitBook

注册/登录 [GitBook](https://www.gitbook.com/), 使用 GitHub 账号登录。

![img](https://camo.githubusercontent.com/5eee99dca1b56c812d05ead5b03128d23b4d9a98/687474703a2f2f69342e7069696d672e636f6d2f3536373537312f333737363765636237623462363839632e706e67)

### 第三步：创建 GitBook

点击 `+New` 新建一本书，在类型里选择 GitHub ，然后选择你要关联的仓库（一般为 Fork 之后生成的个人仓库），然后点击 `create book`。

![img](https://camo.githubusercontent.com/2f7275633003e56bf6f4a015db5e1f21cb49fd84/687474703a2f2f6f70656e6d696e64636c75622e71696e6975646e2e636f6d2f73686172652f4862476974426f6f6b53657474696e675669614769744875622e706e67)

就这样配置成功啦！	现在，你可以在 GitHub 网页/客户端更新你的个人仓库， GitBook 会同时更新。若你在 GitBook 网页端更新你的笔记或作业, GitHub 仓库也会同时更新。

你还可以点击 `PDF/ePub/Mobi` 则可以下载相应格式到本地。

### 如何把私有库用 GitBook 发布？

课程仓库一般为 私有库，你 Fork 后生成的个人仓库也是私有库。

如果想把私有库用 GitBook 发布，需要你授权， GitBook 才可以查找你希望关联的私有库。

处理方式如下：

GitBook Account Setting > GitHub > With access to private repositories ，然后按着提示授权就好：

![img](https://camo.githubusercontent.com/22fd2882ecf00e6b1bed7d7cb8c26cf88ff678f9/687474703a2f2f6f70656e6d696e64636c75622e71696e6975646e2e636f6d2f73686172652f4862476974426f6f6b53657474696e67507269766174655265706f2e706e67)

### 如何添加新内容？

如果你在 GitHub 上添加了新的 MarkDown 文档，需要在 `SUMMARY.md` 中添加新加入文档的路径，这样才能建立目录和新内容的链接，GitBook 的书籍目录才会显示新内容。例如，你在 chapter01 新添加 `new.md` 文档，此时 GitBook 的目录中并不能看到这篇文档。按下图修改 `SUMMARY.md` 之后，就可以了。`SUMMARY.md` 是整本书的目录，增删书籍内容时，不要忘记修改这个文档。

![22](https://camo.githubusercontent.com/f2283e63b5265ae6725dfa1cb3da2e0d59e21579/68747470733a2f2f636c6f75642e47697448756275736572636f6e74656e742e636f6d2f6173736574732f31343834303137302f31333838393937302f32663266666634382d656438342d313165352d396431312d3961303639366533333935632e706e67)

## 给 GitBook 添加评论功能

如果想要获取他人对自己书籍的反馈，那么你可以选择添加评论功能。有两种实现方法：

### 1. Disqus

Disqus 较为稳定且美观，但必须科学上网才能使用。使用方法：

1. 首先在 [disqus.com](http://disqus.com/) 中注册一个账号，登入之后在[此页面](https://disqus.com/profile/signup/?next=/admin/create/)注册一个Disqus页面，记住 `.disqus.com` 之前空白处填写的用户名（shortName）。

2. 修改你 GitHub 仓库中的 book.json 文件（如果没有，请自行用 Atom/ sublime text 等全能编辑器创建该文件，命名为 book.json 即可）。然后把下面的 `your_short_name` 替换成之前注册 Disqus 页面时 `.disqus.com` 前的用户名，保存到 book.json 文件里就可以啦。

   ```
   {
       "plugins": ["disqus"],
       "pluginsConfig": {
           "disqus": {
               "shortName": "your_short_name"
           }
       }
   }
   ```

   配置完成后，回到你的 GitBook，每个内容页下方就会出现 Disqus 评论区。

### 2.多说

多说的好处是速度较快，但没有 Disqus 美观稳定。

1. 登陆[多说 - 社会化评论系统](http://duoshuo.com/)，点击首页的 “我要安装”，创建一个站点。

2. 修改仓库文件 book.json （如果没有，请自行用 Atom/ sublime text 等全能编辑器创建该文件）：

   ```
   {
   	"plugins": [
     "duoshuo"
     ],
     "pluginsConfig": {
     "duoshuo": {
         "short_name": "用户名",
         "theme": "default"
      }
     }
   }
   ```

## 更多内容

以上只是简单的配置指南，如果你遇到更多问题，或者想进一步探索 Gitbook，请参考 [GitBook 官方指南](https://help.gitbook.com/)。

期待见到你的第一本 GitBook！

## CHANGELOG

- 170212 闪闪修订文字错误
- 170124 闪闪更新 DISQUS 配置说明
- 170118 闪闪增补评论插件配置说明
- 170113 闪闪增补目录
- 170109 闪闪根据新版 GitBook 更改配置说明
- 160815 闪闪修订措辞
- 160803 李长宸创建