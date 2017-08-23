# osu!tourney

**osu!tourney** 是 osu! 的官方多人旁观客户端，您可以使用它观看或直播全部多人房间。

如果您遇到问题，可以阅读下面的故障排除部分，也可以发送邮件至 [tournaments@ppy.sh](mailto:tournaments@ppy.sh)。

## 什么是 osu!tourney ？

osu!tourney 客户端是用于旁观在多人房间里所有玩家的官方直播客户端，支持 2 个团队，最多 8 人的直播。

目前，它只是用于 World Cup ，所以行为可能会被限制。

## 设置

**注意：** 要使用 osu!tourney，您需要拥有 supporter 标签。

只需几个步骤即可设置 osu!tourney 客户端。

首先，建议安装一个全新的 osu! 客户端！这是因为歌曲数据库极有可能被破坏。

您可以同时安装多个 osu! 客户端，只需要将它们存放在不同的文件夹即可。
您只需将需要的歌曲添加至您的 `/Songs/` 文件夹中，客户端就会自动开始下载缺失的谱面。
osu!tourney 客户端只支持已经提交的谱面。

1. 安装一个新的 osu!
   如果您要这么做，请先将目录下的 `osu!.exe` 复制到一个新的空文件夹，然后运行它即可。
   它应该会自动开始更新和安装。
2. 打开安装完毕的 osu! 并登录。
   不要忘记选择 **记住用户名** 和 **记住密码**
3. 切换更新版本到 **测试版**。
4. 在这个新的文件夹里创建一个文件名为 `tournament.cfg` 的文件。
5. (重新)启动您的 osu! 客户端，osu!tourney 应该会启动。
   这可能需要一段时间，请耐心等待。
   它将会自动生成 `tournament.cfg` 文件的内容，它将包含以下行：
   
  ```
  TeamSize = 4
  privateserver =
  acronym = Your tournament name
  BufferTotalTime = 3000
  BufferDangerTime = 1000
  BufferTimeoutTime = 20000
  ```

关闭 osu! 然后编辑或添加您的比赛所需选项，下面列出了全部选项。如果没有明确说明，时间均以毫秒为单位：

- `TeamSize` 定义您的团队大小，osu!tourney 可以为每个团队打开 1-8 个窗口，最大值是8。
- `ClientNameSize` 改变黄色玩家的名字大小(通常是Staff)。
- `privateserver` 不要改变这个选项，这和您没关系。
- `acronym` 将您的比赛缩写放在这里，例如 OWC 2013。
  您可以在 ** ** 找到更多的细节。
- `BufferTimeoutTime` 定义超时等待时间，如果超出该时间仍无法缓冲其中某个客户端，客户端将试图继续缓冲，并同步其它客户端继续播放。
- `BufferTotalTime` 定义客户端缓冲的时间以减少等待缓冲的频率，不建议改变这个。
- `BufferDangerTime` The remaining time in the replay buffer before the client pauses to wait for more replay frames.
  It is not recommended to change this.
- `RankingChatDelay` 当xx结束后隐藏分数并在排名屏幕上再次显示聊天的延迟。
- `Height` 客户端高度
  osu!tourney 将自动计算客户端宽度(16:9比例)
  黑色控制面板不包括在高度内，所以您其实需要 1440p 的屏幕来使用 1080p 直播您的比赛。
  默认：720，允许范围：568-1440

如果您修改了 `tournament.cfg` 文件，请重启 osu!tourney，它将更新当前设置。

### 使用 osu!tourney

![osu!tourney Interface](Osutourneymain.png "osu!tourney Interface")

_osu!tourney 客户端的基本界面_

这是 osu! tourney 客户端的界面。
客户端本身的使用非常的简单，屏幕顶部被分为两部分，分别代表了多人房间的两个团队，每个 osu! 被分配到多人房间的一个格子。
这意味着玩家将在房间相应位置的窗口上。

---

![osu!tourney Player Windows](Osutourneywindows.png "osu!tourney Player Windows")

_基于玩家所在的格子，他们被分配到对应的窗口位置_


为了使客户端能正常工作，请确保玩家在多人房间里占据适当的格子。
有关更多正确使用的细节，您可以在 **多人房间创建和处理** 中找到。
在客户端的底部，您将看到控制面板。

---

![osu!tourney control panel](Osutourneypanel.png "osu!tourney control panel")

---

![When the multiplayer rooms are created correctly, they will be listed instead of the instructions](Osutourneyroomlist.png "When the multiplayer rooms were created correctly, they will be listed instead of the instructions")

![osu!tourney assigns team names and usernames automatically](Osutourneyidle.png "osu!tourney assigns team names and usernames automatically")

![osu!tourney does not simply spectate. It also shows the current team score and the currently played song](Osutourneyspectate.png "osu!tourney does not simply spectate. It also shows the current team score and the currently played song")

![osu!tourney declares a winner automatically, adds a score and plays another sprite when showing the results screen. Failed players are blacked out.](Osutourneyresults.png "osu!tourney declares a winner automatically, adds a score and plays another sprite when showing the results screen. Failed players are blacked out.")

它将显示您需要遵循的多人房间命名模板。
它由您在 `tournament.cfg` 里定义的比赛缩写和 2 个团队名称组成。
阅读 **多人房间创建和处理** 以了解更多信息。

控制面板将列出所有正确创建的多人房间，点击您创建的多人房间，osu!tourney将会自动开始旁观。

当谱面结束后，osu!tourney 将给获胜队伍加一颗星以增加队伍得分。
**您还可以通过左键单击以增加或右键单击以减少来手动改变队伍得分**

![osu!tourney with activated annotation](Osutourneywarmup.png "osu!tourney with activated annotation")

如果要显示自定义信息，可以单击 annotation 按钮来切换。
当处于激活状态时，相应信息将显示在屏幕顶部，谱面结束后的得分将保持不变。

底部控制面板描述：

- `Sync music`: 如果音乐处于不同步的状态，您可以试图单击此按钮，osu!tourney 将尝试将音乐重新和击打音效同步。
- `Toggle annotation`: 激活/取消激活自定义信息的显示，这将影响队伍得分计算。
- `Panic`: 出现问题时请试图单击此按钮，例如：一个窗口没有观察到用户或窗口崩溃，这将重新初始化所有窗口。
- `Exit`: 关闭 osu!tourney

底部控制面板文本框描述：

- `Annotation text`: 自定义信息的文本
- `Best Of`: 每个队伍需要赢得的谱面数量

## 多人房间创建和处理

### 创建房间

要使 osu!tourney 能正常的在您创建的房间运作，您必须注意几件事情。

您必须根据 osu!tourney 控制面板列出的模板创建一个多人房间。
此模板包括：

`Your_acronym_in_tournament.cfg: (Team Name 1) vs (Team Name 2)`

`Your_acronym_in_tournament.cfg` 您可以在 `tournaments.cfg` 里改变比赛的简称。
在我们的例子中，这个简称为 "Test Tourney"。

`Test Tourney: (Team Name 1) vs (Team Name 2)`

您可以使用您的队伍名称替换 "Team Name 1" 和 "Team Name 2"，不过请在其周围保留括号。

### 房间管理

您可以在此查看更多信息 [Tournament Management Commands](/wiki/Tournament_Management_Commands "Tournament Management Commands")。

osu!tourney 客户端将成功识别房间。
确保使用 !mp move 和 !mp team 命令为玩家分配合适的队伍和格子。

正如 **using osu!tourney section above** 所述，客户端的每个窗口都分配给相应位置的格子。
根据您在 `TeamSize` 中定义的值，左侧的队伍将占据 the left team will occupy the first slots and the right team will occupy the slots right below that.

![osu!tourney Player Assignment](Osutourneyassignment.png "osu!tourney Player Assignment")

_相应的格子在 osu!tourney 对应到的窗口_

在例子里，如果您设置了 `TeamSize = 4`，第 1/2/3/4 个格子将在左侧的队伍。
第 5/6/7/8 个格子将在右侧的队伍。

如果您设置了 `TeamSize = 3`，第 1/2/3 个格子将在左侧的队伍。
第 4/5/6 个格子将在右侧的队伍。

**提示：为了更容易参考，总是让左侧的队伍变蓝，右侧的队伍变红。**

请记住，osu!tourney 忽略每个团队的颜色。
唯一有关的仅仅是多人房间的格子。

为了让每个玩家都能在 osu!tourney 的正确队伍内进行，玩家必须占据多人房间内的正确位置。以下是不同团队规模的 osu!tourney 的图片，屏幕上的数字表示多人房间里为玩家分配的格子，这些数字在 osu!tourney 中是不可见的，仅仅是因为描述而放在这里。

![TeamSize = 4](Osutourneywindows.png "TeamSize = 4")

---

![TeamSize = 3](Teamsize3.png "TeamSize = 3")

---

![TeamSize = 2](Teamsize2.png "TeamSize = 2")

---

![TeamSize = 1](Teamsize1.png "TeamSize = 1")

### 皮肤

![osu!tourney can be customized in various ways](Osutourneycustom.png "osu!tourney can be customized in various ways")

osu!tourney 支持使用皮肤进行自定义修改，您可以设计并应用适合您的比赛的客户端。
为此，您需要在您的 osu!tourney 目录下创建 `Skin` 文件夹。

皮肤的放置路径必须是 `/osu!/Skins/User/tournament`。
皮肤可以放在该文件夹里，支持 .jpg 或 .png 文件扩展名。
要正确应用您的皮肤，请相应的命名这些文件：

- `background` - 这是 osu!tourney 使用的背景。默认背景可以在 [这里](https://s.ppy.sh/images/tournament/default.png) 找到。
- `background-win1` (可选) - the background sprite will be fade over to this sprite in Results Screen when the left team won.
   It will fade back to `background` when leaving Results Screen.
   If this element is not placed, it will stay on `background`.
- `background-win2` (可选) - the background sprite will be fade over to this sprite in Results Screen when the right team won.
   It will fade back to `background` when leaving Results Screen.
   If this element is not placed, it will stay on `background`.
- `tourney-title` (可选) - this image will be placed placed on top of your background sprites and will be located at the bottom of your osu!tourney screen.
   这可以用于放置静态图像，例如您的比赛标志。

![osu!tourney with team icons. The left icon is named Team 1.png and the right icon is named Team 2.png](Osutourneyicons.png "osu!tourney with team icons. The left icon is named Team 1.png and the right icon is named Team 2.png")

您可以在皮肤文件夹创建您的团队图标(国家图标或玩家头像)。
这些图标必须放置在该路径：`/osu!/Skins/User/tournament/icons`.

所有图标必须与队伍名称完全相同。
如果您的房间叫 `Test Tourney: (Team 1) vs (Team 2)`，则您的图标必须命名为 `Team 1 和 Team 2`。
图标可以使用 `.jpg` 或 `.png` 格式和 `50x50px` 的最佳分辨率。

[下载皮肤模板](https://s.ppy.sh/images/tournament/template.zip)以快速创建您的皮肤

### 奖品

我们可以奖励profile badges给比赛符合以下标准的第一名获胜者：
- 这是比赛的第二
- 比赛 Staff 不参与比赛本身
- 比赛每年举办四次或更少(季节性)

如果您的比赛符合这个标准，请通过邮件联系 tournaments@ppy.sh。

## Troubleshooting

### How do I create a fresh osu! installation without uninstalling the current game?

Copy `osu!.exe` into an empty folder and run it.

### My osu! windows are not aligning properly!

Disable any **secondary monitors!**
osu!tourney only runs on the primary monitor. Try disabling any secondary monitors you have active. Make sure that the primary monitor has a resolution larger than the resolution of the client (1280x720 by default).

Ensure that you did **not** run osu! as administrator (unless osu! is asking for it directly on its own).
Make sure to have osu! updated to the newest cuttingedge build!

### osu!tourney does not open, it throws me an error prompt and/or closes!

- Ensure that osu! is using the Cutting Edge release stream.
- Make sure that you are logged into osu! If not, run osu! normally, login while making sure the "Remember Username" and "Remember Password" checkboxes are checked, then restart osu! as the tournament client.
- Ensure that the `privateserver` key in `tournament.cfg` has no value set.

### My osu! song database corrupts when starting up!

Use a fresh osu! installation.

### The background of the osu!tourney is not shown!

Make sure your background file is properly located at `/osu!/Skins/User/tournament/background.png`.
See the **Skinning** section for more details.

### How do I make osu! run as a normal client again?

Rename or delete the `tournament.cfg` file.

### My client is not spectating!

Make sure you have **joined the room!**

Click the room name on the bottom black panel until it is **bold**.
If the client is still not spectating, click the `Panic` button.

### The rooms are not showing up!

It is possible that your multiplayer room is named incorrectly or you used the wrong acronym in `tournament.cfg`.
Make sure you are using the correct room name (see the **Match Creation** section), renaming an existing multiplayer room will not work.
If the above doesn't work, recreate the room while following the **Match Creation** section of this guide closely.

Email [tournaments@ppy.sh](mailto:tournaments@ppy.sh) if you require further assistance.

### The team names are not showing!
See previous answer.

### How do I stream my tournament to streaming services like Twitch?

To set up a stream, we recommend using the [Open Broadcaster Software](https://obsproject.com/), but know that you are also free to use any other streaming client you have access to.
The resolution of the top part of osu!tourney can be customised but by default it is `1280x720`. Make sure that the resolution of your monitor is bigger than this value. See the Setup section for information on how to change the resolution.
Do not forget to adjust the cropping to remove the black control panel from the stream!

### My issue/question is not listed here! What to do?

Email tournaments@ppy.sh if you have a problem that is not listed here. Make sure to be descriptive and provide screenshots if possible.
