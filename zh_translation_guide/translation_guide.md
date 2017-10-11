# osu 中文翻译指南

![[Discord链接](https://discord.gg/Gud9s9z)](https://discordapp.com/api/guilds/281826842657161216/widget.png?style=banner2)

## 组织介绍

![shield](https://img.shields.io/badge/organization-osu!translate%20zh-blue.svg?style=flat-square)

osu-translate-zh（osu!中文翻译组织）是由玩家自发参与和贡献的翻译组织，负责 osu! 官方中文翻译工作。

翻译的内容包括 `osu!lazer`，`osu-web` 和 `osu-wiki`。其中：

- `osu!lazer` 正在开发中，i18n（国际化）相关的功能未完成，客户端的翻译工作将会在这些功能完成后开始。
- `osu-web` 目前官网页面的翻译与开发进度保持一致，会以每个月补丁的形式增加新的翻译或者修订已有的翻译。
- `osu-wiki` 是翻译工作的重点，Wiki 中有大量新增的内容和大量过时的内容需要翻译，精简，修订和补充。

翻译的语言包括简体中文（zh），繁体中文（zh-tw），其中也包括粤语（zh-hk）。

翻译组织的大部分成员来自大陆，因此简体中文的翻译是最先进行的。

~~在繁体中文负责人被提名前，简体中文的文章会用工具转换为繁体，再通过人工审阅的方式修订最终的翻译。~~

粤语相关的翻译问题正在讨论中。

*****

为了相互交流和协作，翻译出高质量的内容，我们成立了 osu!中文翻译组织。

我们希望能提供和谐的讨论环境，准确和恰当的翻译参考，高效率地进行翻译工作。

osu!中文翻译组织 欢迎**任何人**参加到翻译工作中，特别是有 Wiki 翻译经验或者对 osu! 有相当程度的了解的玩家。

如果你没有这方面的特长，请不用担心，你也可以加入我们贡献一份的微薄之力，我们会安排合适你的相对轻松的工作。

## 工作流程

### 面向初次使用 github 的人

（介绍 web 上的审阅和翻译流程）

### 面向对 github 非常熟悉的人

（介绍使用 git 的翻译流程）

在介绍 osu! 中文翻译的翻译流程之前，我们假定你对 Git（分布式版本控制软件）和 Github（代码托管平台）有一定的了解。具体要求如下：

- 创建了自己的 Github 账号。（**必须**）
- 理解 Github 的工作流（Workflow）。
- 电脑上安装了 Git 。（**非必须**）
  - 会使用 `git commit`，`git fetch`，`git checkout` 这些常用命令。

如果没有的话，请参阅下面的链接，一步步学习如何使用 Git 和 Github。

<!-- git-scm book和廖雪峰博客 -->
(TODO: some urls)

虽然它们看起来很高大上，甚至很复杂，但是学习它们带来的收益是巨大的，可以给极大的效率提高工作效率。

### 审阅流程

Reviewer 身份组的工作是审阅别人的翻译，留下自己的意见和建议。这与一般的 Review 工作流没有区别。

你可以在 osu-translate-zh 的 [Pull Request 列表](https://github.com/osu-translate-zh/osu-wiki/pulls) 中查看需要 Review 的 PR。

在 PR 中点击某个特定的 Commit 或者点击 `Filed changes`，即可看到相关的修改。

鼠标移动到某行上，直接点击即可输入自己的评论（Comment）。

输入后请点击 `start review` 或 `add review comment`。

完成审阅后，点击评论框中的 `Finish your review`，在右上角的文本框中输入总结性的评论，最后点击 `Submit review`，即完成了一次 Review。

### 翻译流程（web）

<!-- WIP -->

### 翻译流程（git）

Translator 身份组的工作是翻译 Wiki 中的文章。

翻译流程的几个关键点是：

- 翻译的 Pull request 是由自己的仓库到组织的仓库，当我们在组织内 Review 完成这篇翻译后，再从组织仓库 Pull request 到 ppy 仓库。

这是为了将中文和其他的语言的翻译 PR 分开，互不干扰，以及自由地使用中文进行评论。

- 接下一篇翻译任务时，请在组织内新建一个对应的分支，这篇翻译的 Pull request 的目标分支请设置为这个分支。

因为一篇文章对应于一个分支，翻译完成后我们会将组织中的这个分支 Pull request 到 ppy 仓库。
（TODO: 关于权限的说明。）

- 翻译之前，请文件夹中复制一份 `en.md` 文件，并改名为 `zh.md`，并作为第一个 Commit（Commit 信息为 `zh: Init translation`）。
这是为了方便以后 Review 的时候可以直接对照原文，例如：

<!-- 改用github的图床 -->
![files changed](https://wx3.sinaimg.cn/large/006fVPCvly1fkcdzfxfcej30c303aglo.jpg)

比如，你想翻译 `Guides` 页面，需要先在组织中建立一个 `zh-guides` 分支，然后 Fetch 组织仓库，新建一个本地分支，翻译文章，最后 Push 到自己的仓库中，Pull request 到组织仓库中。

下面详细讲解翻译流程：
1. Fork 组织仓库。在 [osu-translate-zh/osu-wiki](https://github.com/osu-translate-zh/osu-wiki) 页面的右上角点击 Fork 即可。

2. Clone 自己的仓库到本地。执行 `git clone <你的仓库的 git url>` 命令。
自己仓库的 Git url 可以在自己仓库的页面上找到。

![clone url](https://wx2.sinaimg.cn/large/006fVPCvly1fkc5dzdh3dj30ag0760sz.jpg)

3. 在组织仓库中建立新的分支 `zh-guides`。

![create branch](https://wx4.sinaimg.cn/large/006fVPCvly1fkcdtuddqaj308i07g74e.jpg)

4. Fetch 组织仓库，新建一个本地分支。
```
git remote add zh https://github.com/osu-translate-zh/osu-wiki.git
git fetch zh
git checkout -b zh-guides zh/zh-guides
```

5. 现在你可以进行翻译工作，完成后进行 Commit，然后执行 Push 命令提交到自己的仓库。
```
git add .
git commit -m "update zh.md"
git push -u origin zh-guides
```

6. 从自己的仓库 Pull request 到组织仓库。注意两个分支相对应。

7. 进行 Review 工作，最后这个分支会被合并进组织的 `zh-guides` 分支中。

8. 去 ppy 仓库 Pull request 这个分支。一般会很快被合并进 Master 分支。

### 接管（甩锅）流程

某些时候，原来的翻译者无法继续进行翻译，需要新的翻译者来继续未完成的翻译工作，应当这么做：
1. 合并原来的未完成的 Pull request。
2. 新翻译者 Fetch 组织仓库，在本地创建新的分支，继续进行翻译。
3. 将这个本地分支推送到自己的仓库中，并 Pull request 到组织仓库。
4. 按照正常的翻译流程继续进行。

## 翻译指南

### 规则 Rules

<!-- WIP -->

### 文章风格指南 ASC

ASC 由 [@kj415j45](https://github.com/kj415j45) 负责翻译。目前 en 版本已未完成，中文翻译正在进行中。

### 名词对照表

目前正在整理中，参见：

[osu! 中文翻译 名词对照表](https://docs.google.com/spreadsheets/d/1zhUP0qekKRUWb1Mu-P89mwu_HcPBen5FoGPqD2MkI7k)

## github 贡献指南

### Commit message 规范

请按照以下面的四个句子作为 Commit message：

1. `zh: init translation` 第一个 commit。

复制 `en.md` 并重命名为 `zh.md`。

2. `zh: 英文的文章标题` 完成了部分翻译。

可以重复使用多次这句 Commit message。但是，太多的话会被 Squash 成一次 Commit。

当某篇 Wiki 包含子页面时，请使用 `-` 符号连接，写上完整的标题。例如： `Ranking_Criteria - osu!catch`

3. `zh: apply reivews` 根据 review 修改一些翻译语句。

4. `zh: finish 英文的文章标题` 完成了所有翻译。

这句作为最后的 commit，也作为 merge commit。

### Pull request 规范

PR 命名和内容都没有特别的要求，中文英文均可，只要能清楚的表达意思就行。

## 相关链接

[osu! 中文翻译 名词对照表](https://docs.google.com/spreadsheets/d/1zhUP0qekKRUWb1Mu-P89mwu_HcPBen5FoGPqD2MkI7k)

[osu!wiki 中文翻译 进度表](https://docs.google.com/spreadsheets/d/1zjXM0BAWA-bYDGcxPUlysO_G3IZcbsQJ9c8fv_7OOeY)

[osu!wiki 中文翻译 任务表](https://github.com/orgs/osu-translate-zh/projects/1)

[osu!wiki 翻译完成进度](https://github.com/osu-translate-zh/osu-wiki/issues/1)
