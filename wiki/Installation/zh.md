Installation (中文)
======================

安装指南
-------

此页面会告诉你如何获得游戏和一些排除故障的方法。

### 桌上型电脑

#### Windows 系统

##### 最低系统要求
- 1 GHz 以上的中央处理器
- 512 MB 以上的内存
- [Microsoft .NET Framework 3.5以上](https://www.microsoft.com/zh-cn/download/details.aspx?id=22)

##### 如何安装
- 下载 [osu! 安装程序](https://osu.ppy.sh/p/download)。
- 找到刚刚下载的文件，双击它，然后按照说明安装 osu!。
- 双击创建在桌面的 osu! 图标，它位于你的桌面或开始菜单。
- 主菜单应会显示出来。你应该登录来玩 osu!（通过单击相应的按钮创建一个)，但是你也可以离线玩 osu!。（所有的成绩将不会提交到数据库）。
  - 在线模式会计算你的分数，表现以及全球排名。
- 享受你的 osu! :)

##### 添加谱面
谱面（osz 文件）是包含歌曲和播放所需要的文件。
- 你可以前去 [谱面列表](https://osu.ppy.sh/p/beatmaplist). 找一个你喜欢的谱面，点击它的标题，打开其歌曲的网页。
- 然后在网页上登录。
- 单击粉色的下载（Download）按钮。
- 如果你想下载不包括视频的谱面，单击紫色的 No Video 按钮。
- 有几种方式可以导入谱面文件：
  - 如果系统或浏览器询问你：“如何打开此 osz 文件？”，您应该选择“打开方式：osu!”，osu! 会自动打开并导入文件。
  - 如果您选择保存文件，或者您的浏览器不允许你选择打开方式，你可以进入下载目录，然后双击它，osu! 将会自动导入。
  - 如果 osu! 已经打开，你也拖动 osz 文件到游戏窗口上，然后松开，osu! 将会自动导入。你也可以将你的 osz 文件放置在 osu! 目录的“Song”文件夹。
- 现在你就可以玩你的谱面啦！如果列表中没有出现你导入的谱面，只需在歌曲菜单按下 F5 键，列表会自动刷新。
- 你也可以下载 **[beatmap 包](http://osu.ppy.sh/p/packlist)** ，beatmap 包是把一些谱面整合。它们一般都是 zip 或 rar 文件。你可以下载一个你喜欢的压缩程式提取它（例如 [7-Zip](http://www.7-zip.org/)），并导入提取出的 osz 文件。
- 如果你知道如何使用 BitTorrent 客户端，你可以使用 [由社区成员提供的 torrent 文件](https://osu.ppy.sh/forum/t/147478)，这可以让你一次下载许多 beatmap 包。

#### Linux (利用 Wine)
>这个教程可能不是最新的，你可以通过在论坛查看[这个帖子的最后一页](http://osu.ppy.sh/forum/t/14614)找到安装最新 osu! 的方法。

##### 如何安装

1. 基本安装。
  - 首先，检查你的显卡.
    - 使用 NVIDIA 显卡以获得最佳游戏体验。
    - 如果你使用 Intel 显卡，你需要启用 V-Sync。
    - 对于 AMD HD**** 系列显卡 ，你需要关闭 shaders。
  - 安装"Wine"（如果你还没有安装的话）.

2. 使 Wine 工作
  - 对于 Ubuntu/GNU/LINUX Debian, 在终端输入以下指令：
    - sudo apt-get -y install wine
  - 对于 Gentoo / Sabayon：
    - sudo emerge wine
  - 对于 Fedora：
    - sudo yum install wine
  - 对于其它发行版，请阅读相应文档。
  - 创建 Wine 启动参数
    - mkdir ~/.wine-osu
    - cd ~/.wine-osu
    - export WINEPREFIX=~/.wine-osu WINEARCH=win32
    - winecfg
请记住，如果你想启动/安装 osu! 或设置 Wine Prefix，请按照以上流程进行修改。

3. 让osu! 运行起来。
  - 你需要使用 winetricks（wine的一个辅助工具），你可以在终端输入以下指令来安装它
    - winetricks install dotnet20 ie7
  - 下载 osu! Windows 的最新版本。
  - 安装 osu!。
- 启动 osu!。

##### 添加谱面
- 从文件管理器拖放 osz 文件到 osu! 游戏窗口上，osu! 将会自动导入。
