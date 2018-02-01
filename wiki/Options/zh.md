# 设定

![设定菜单](img/options_basic.jpg "设定菜单 \(左侧的侧边栏\)")

点击`设定`，在主界面按`O`或者在几乎任何界面按`Ctrl` + `O`即可访问设定菜单并修改 _osu!_ 的设置。

在这里，直接输入即可搜索你想修改的设定。
如果搜索内容有误，搜索栏的文字会*抖动*且无法输入错误的字符。

当你修改一个含有默认值的设定时，在左侧的灰色竖条会亮成黄色。
点击黄色竖条即可恢复默认值。

## 常规

![常规图标](img/general.jpg "常规图标")

这部分包含你的账户、语言设置、以及你想获得哪种osu!客户端的更新。

### 登录

如果你未登录osu!客户端，游戏会自动弹出设定菜单提示你登录。
你可以按`Esc`，点击返回按钮或者前往歌曲选择界面来忽略。
未登录的状态下，osu!客户端将把你标记为 "来宾" 且你将无法获取在线成绩或进行[多人游戏](wiki/Multi)。

如果你是一位来宾，你会看到以下设定：

|     名称     |                                   用途                                    |  类别  | 默认值 |
| ------------ | ------------------------------------------------------------------------- | ------ | ------ |
| `用户名`     | 输入你的 _osu!_ 用户名。                                                  | 文本   | (空)   |
| `密码`       | 输入你关联 _osu!_ 用户名的密码。                                          | 文本   | (空)   |
| `记住用户名` | 如果勾选，此osu!客户端会记住你的用户名。                                  | 复选框 | `开启` |
| `记住密码`   | 如果勾选，此osu!客户端会记住你的密码。                                    | 复选框 | `开启` |
| `登录`       | 开始登录。你也可以在用户名或密码栏中按`Enter`。                           | 按钮   |        |
| `创建账户`   | 用你的默认浏览器将你重新定向至[创建账户](https://osu.ppy.sh/p/register)。 | 按钮   |        |

---

如果你已经登录，你会看到：

|          名称          |                 用途                 | 类别 |
| ---------------------- | ------------------------------------ | ---- |
| `哈喽，{用户名}。欢迎来到osu!` | 显示一个含有四个按钮的对话框，如下。 | 按钮 |

---

如果你点击`哈喽，{用户名}。欢迎来到osu!`提示框，它会弹出一个对话框：

|      名称      |                      用途                      | 类别 |
| -------------- | ---------------------------------------------- | ---- |
| `查看个人资料` | 在osu!网站上浏览自己的个人资料。               | 按钮 |
| `注销`         | 从此osu!客户端中注销。                         | 按钮 |
| `修改头像`     | 修改你的用户头像。（你将被重新定向至osu!网站） | 按钮 |
| `关闭`         | 关闭对话框。你也可以按`Esc`。                  | 按钮 |

你也可以在任何含有玩家名片的界面访问此对话框。

### 语言

|          名称          |                                      用途                                       |   类别   | 默认值 |
| ---------------------- | ------------------------------------------------------------------------------- | -------- | ------ |
| `语言`             | 显示语言列表。你可以点击你想使用的语言。                                        | 下拉菜单 |        |
| `以原语言显示歌曲信息`   | 谱面会显示他们的"原本"的未经翻译的语言数据，如果可用。                          | 复选框   | `关闭` |
| `聊天窗口使用Tahoma字体` | 在[聊天窗口](/wiki/chat console)使用旧字体（Tahoma）来替代当前字体（Aller）。 | 复选框   | `关闭` |

### 更新

|       名称       |                       用途                       |   类别   |     默认值     |
| ---------------- | ------------------------------------------------ | -------- | -------------- |
| `更新版本`       | 显示你可以使用的一系列版本。                     | 下拉菜单 | `正式版（每月更新）` |
| `osu!已经是最新版！` | 强制使osu!客户端重新检查更新，并下载他们。       | 按钮     |                |
| `打开osu!所在文件夹` | 打开本地 _osu!_ 文件夹。（包含你的皮肤、谱面等） | 按钮     |                |

---

如果你打开了`更新版本`的下拉菜单，你会有以下设定供选择：

|             名称              |                     用途                      |
| ----------------------------- | --------------------------------------------- |
| `正式版（每月更新）`                | 公共发布版本。                                |
| `候选版（每周更新）`                        | 开发者版本 - 早些获得新功能，但是问题比较多。 |
| `测试版（不定期更新）` | 开发者版本 - 更早获得新功能，但是问题会更多。 |

## 画面

![画面图标](img/graphics.jpg "画面图标")

这部分是关于osu!客户端和部分界面的设置。

### 渲染器

|      名称       |                               用途                               |   类别   |  默认值  |
| --------------- | ---------------------------------------------------------------- | -------- | -------- |
| `帧数限制`       | 修改帧数限制。参阅下方内容。                                      | 下拉菜单 | `120FPS` |
| `显示帧数（FPS）` | 在屏幕右下方可见FPS计数器。                                      | 复选框   | `关闭`   |
| `兼容模式`      | 使用 _osu!_ 在旧操作系统的的旧渲染方式。这会重启你的osu!客户端。 | 复选框   | `关闭`   |
| `减少丢帧`      | 感觉经常丢帧的玩家可尝试勾选，调节图像设置来降低丢帧，但是会轻微降低帧数。                                         | 复选框   | `关闭`   |
| `检测性能问题`  | 当其他在你计算机上的软件影响osu!客户端的性能时警告你。           | 复选框   | `开启`   |

---

如果你打开了`帧数限制`的下拉菜单，你会有以下设定供选择：

|        名称        |                                   用途                                   |
| ------------------ | ------------------------------------------------------------------------ |
| `垂直同步`         | 将osu!客户端的刷新频率与你的显示器刷新频率同步。更多内容请查看下方说明。 |
| `120fps`           | 将osu!客户端的刷新频率限制在120FPS。                                     |
| `240fps`           | 将osu!客户端的刷新频率限制在240FPS。                                     |
| `无限制（游戏中）` | 将osu!客户端的刷新频率与你的显示器刷新频率同步。更多内容请查看下方说明。 |

- `垂直同步`说明：通俗来说，使用垂直同步会强制让osu!客户端在显示之前等候完整的一帧。
  - 如果你发现了屏幕撕裂（当游戏下半部分和上半部分不同步），你可能会想使用它。
  - 尽管如上述所述，这么做会导致延迟或缓慢因为osu!客户端必须等待每一帧来加载。
- `无限制（游戏中）`说明：仅会在你游戏谱面时无限制fps。
  - 当你不在游戏谱面时会使用`240fps`。

对笔记本用户的警告：使用`无限制（游戏中）`可能会导致你的笔记本过热！请记住，FPS限制越高，osu!客户端就会消耗更多资源！

注：当osu!客户端不是活跃窗口时，FPS会自动限制到30。

### 屏幕分辨率

|     名称     |                                      用途                                      |   类别   | 默认值 |
| ------------ | ------------------------------------------------------------------------------ | -------- | ------ |
| `分辨率`     | 改变游戏界面分辨率。不同的显示器，下拉菜单提供的设定不同。                     | 下拉菜单 |        |
| `全屏模式`   | 全屏osu!客户端（降低输入延迟）。                                               | 复选框   | `关闭` |
| `不缩放画面` | 用所给分辨率全屏osu!客户端（降低输入延迟）并用黑边框将游戏限制在屏幕中央部分。 | 复选框   | `开启` |
| `水平位置`   | 调节宽屏幕模式的水平偏移。只有在`宽屏幕模式`下才会体现。                       | 滑条     | `0%`   |
| `垂直位置`   | 调节宽屏幕模式的垂直偏移。只有在`宽屏幕模式`下才会体现。                       | 滑条     | `0%`   |

- 若`全屏模式`关闭，`注意：非全屏模式下可能会有输入延迟！`的警告会在其下方显示。

### 详细设置

|        名称         |                                                用途                                                |   类别   |        默认值         |
| ------------------- | -------------------------------------------------------------------------------------------------- | -------- | --------------------- |
| `渐出滑条`   | 滑条从起始点逐渐滑出。                                       | 复选框   | `开启`                |
| `背景视频`  | 启用背景视频播放。        | 复选框   | `开启`                |
| `Storyboards`       | 在游戏中的背景显示Storyboard。                            | 复选框   | `开启`                |
| `连击提示图`      |当连击数达到一定数值时，屏幕边缘将弹出一个任务图像。  | 复选框   | `开启`                |
| `击打闪光`      | 在击打提示后方加上一个轻柔的闪光。不会在Kiai关闭。              | 复选框   | `开启`                |
| `着色器效果`           |在游戏中启用着色器特效。如果显卡不支持，此选项将被自动禁用。| 复选框   | `关闭`                |
| `柔化滤镜`  |启用柔化滤镜。启用后会自动启用着色器效果。     | 复选框   | `关闭`                |
| `截图格式` | 设置截图文件的格式为`JPEG （空间较小）`或`PNG（无损）`。                      | 下拉菜单 | `JPEG (空间较小)` |

### 主菜单

|          名称          |                                                                         用途                                                                          |   类别   |   默认值    |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- | -------- | ----------- |
| `飘雪效果`                 | 在主菜单添加飘雪效果。（冬季强制开启）  | 复选框   | `关闭`      |
| `视差效果`             | 背景画面会随着光标位置而移动。（不在谱面中适用）| 复选框   | `开启`      |
| `显示提示`            | 在主菜单显示osu!用法小提示。（提示将不会在测试版中显示）       | 复选框   | `开启`      |
| `问候语`     | osu!将在打开和关闭的时候播放问候语。| 复选框   | `开启`      |
| `osu!主题音乐`     | 启动osu!时，主题曲将会播放。一旦歌曲切换，你只能重启osu!来重新播放它。| 复选框   | `开启`      |
| `季节性背景` | 在主菜单（和没有背景的谱面）用同人绘画比赛获胜的背景。会在歌曲改变时轮流切换。  | 下拉菜单 | `有时` |

---

如果你打开了`帧数限制`的下拉菜单，你会有以下设定供选择：

|    名称     |                                                                                            用途                                                                                             |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `有时` | 你会在每个季节开始时看到季节性背景。osu!小队会决定何时取消并换回熟悉的背景。|
| `永不`     | 你永不会看到季节性背景。这代表你将不会看到任何动漫。  |
| `常开`    | 你将一直看到该季节的背景。    |

### 选歌页面

|       名称        |                                                   用途                                                   |  类别  | 默认值 |
| ----------------- | -------------------------------------------------------------------------------------------------------- | ------ | ------ |
| `显示缩略图` | 显示谱面背景图的预览。需要2.2+版本的皮肤支持。| 复选框 | `开启` |

## 游戏

![游戏图标](img/gameplay.jpg "游戏图标")

This section is about the appearance during gameplay.
这部分是关于游戏时的界面设置。

### 常规

|                      名称                       |                                                         用途                                                          |   类别   |      默认值       |
| ----------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- | -------- | ----------------- |
| `背景暗化`                                | 调节游戏时对背景的暗化程度。（适用于背景视频和Storyboards）| 滑条     | `30%`             |
| `进度条位置`                              | 设置在哪里显示歌曲进度。详情见下。| 下拉菜单 | `右上角(饼状)` |
| `Score meter type`                              | Configure accuracy meter appearing below the beatmap. Note that osu!catch will always use `Colour`.                   | 下拉菜单 | `Hit error`       |
| `Score meter size`                              | Configure size of score meter.                                                                                        | 滑条     | `1x`              |
| `Always show key overlay`                       | Show the key status overlay even while playing normally.                                                              | 复选框   | `关闭`            |
| `Show approach circle on first "Hidden" object` | When playing with the "hidden" mod，show only the first note's approach circle.                                       | 复选框   | `开启`            |
| `Scale osu!mania scroll speed with BPM`         | Adjust speed of osu!mania's scrolling depending on the BPM of the beatmap.                                            | 复选框   | `开启`            |
| `Remember osu!mania scroll speed per-beatmap`   | Remember the scroll speed you personally set per-beatmap.                                                             | 复选框   | `开启`            |

---

If you open the dropdown list for `Progress Display`，you will be presented with these options:

|       名称        |                                                                     用途                                                                      |
| ----------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| `Top-Right (Pie)` | Use a pie chart to show the remaining duration before the song starts and the time left before completion. This is seen left of the accuracy. |
| `Top-Right (Bar)` | Use a short horizontal bar to display the time left before completion. This is seen underneath the score but above the accuracy.              |
| `Bottom-Right`    | Use a short horizontal bar to display the time left before completion. This is seen in the bottom-right corner.                               |
| `Bottom (long)`   | Use a long horizontal bar to display the time left before completion. This is seen on the bottom.                                             |

---

If you open the dropdown list for `Score meter type`，you will be presented with these options:

|    名称     |                                            用途                                            |
| ----------- | ------------------------------------------------------------------------------------------ |
| `None`      | Do not use a meter to display the player's hit timing.                                     |
| `Colour`    | Use coloured blocks to display hit timing. (osu!catch uses this if `Hit error` is used.)   |
| `Hit error` | Use a meter to display hit timing. This shows if the player had hit too early or too late. |

### Song Select

|          名称           |                                   用途                                    | 类别 | 默认值 |
| ----------------------- | ------------------------------------------------------------------------- | ---- | ------ |
| `Display beatmaps from` | This adjusts the **minimal** star rating a beatmap needs to be displayed. | 滑条 | `0`    |
| `up to`                 | This adjusts the **maximum** star rating a beatmap needs to be displayed. | 滑条 | `10`   |

## Audio

![Audio 图标](img/audio.jpg "Audio 图标")

This section is about audio related things.

### Devices

|      名称       |                                                用途                                                |   类别   |  默认值  |
| --------------- | -------------------------------------------------------------------------------------------------- | -------- | -------- |
| `Output device` | Select the preferred output device for audio. (Options given based on what your computer reports.) | 下拉菜单 | `默认值` |

### Volume

|            名称            |                                           用途                                            |  类别  | 默认值 |
| -------------------------- | ----------------------------------------------------------------------------------------- | ------ | ------ |
| `Master`                   | Controls all aspects.                                                                     | 滑条   | `100%` |
| `Music`                    | Affects only the music.                                                                   | 滑条   | `80%`  |
| `用途`                     | Affects things such as hit sounds and in-game sounds.                                     | 滑条   | `80%`  |
| `Ignore beatmap hitsounds` | Favor hitsounds supplied by the current skin instead of the beatmap's included hitsounds. | Button | `关闭` |

### Offset Adjustment

|        名称        |                                            用途                                            | 类别 | 默认值 |
| ------------------ | ------------------------------------------------------------------------------------------ | ---- | ------ |
| `Universal offset` | The offset (in milliseconds) that all beatmaps will use (in addition to the local offset). | 滑条 | `100%` |
| `Offset wizard`    | Opens the offset wizard.                                                                   | 滑条 | `80%`  |

- For details about the offset wizard，see [Offset Wizard](/wiki/Offset_Wizard).
- For details on using the offset wizard，see [How to use Offset Wizard](/wiki/How_to_use_the_Offset_Wizard).

## Skin

![Skin 图标](img/skin.jpg "Skin 图标")

This section is about skin related things.

### Skin

|                    名称                    |                                                                  用途                                                                   |   类别   |  默认值  |
| ------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------- | -------- | -------- |
| `Skin sample image`                        | Display various gameplay elements from the selected skin. Click to cycle through different element sets.                                | Button   |          |
| `Current Skin`                             | Change the skin. Items in dropdown is based on what is in the `skin/` folder. (名称s are based on folder name.)                         | 下拉菜单 | `默认值` |
| `Preview gameplay`                         | Preview the skin by playing a random beatmap with auto mod. Mode is determined on what was selected in song select.                     | Button   |          |
| `Open current skin folder`                 | Open the directory the current skin is stored in.                                                                                       | Button   |          |
| `Export as .osk`                           | Export the current skin as a `.osk` file. Once your osu!客户端 is done exporting，it will the directory containing the `.osk` file.     | Button   |          |
| `Ignore all beatmap skins`                 | Favor the selected skin over the beatmap's included skin. This does not include hitsounds.                                              | 复选框   | `关闭`   |
| `Use skin's sound samples`                 | Always use the selected skin's hitsounds instead of the beatmap's included hitsounds.                                                   | 复选框   | `开启`   |
| `Use Taiko skin for Taiko mode`            | Use osu!taiko-specific skin elements，if supplied by the selected skin. See [Skinning/osu!taiko](/wiki/Skinning/osu!taiko) for details. | 复选框   | `关闭`   |
| `Always use skin cursor`                   | Favor the current skin's cursor over any pack-in cursors supplied by beatmaps.                                                          | 复选框   | `开启`   |
| `Cursor Size`                              | Adjust the cursor size.                                                                                                                 | 滑条     | `1x`     |
| `Automatic Cursor Sizing`                  | Automatically adjusts the cursor size based on the circle size of the played beatmap.                                                   | 复选框   | `关闭`   |
| `Use combo colour as tint for slider ball` | 滑条 balls will use the current combo color (usually transparent). Requires skin support.                                               | 复选框   | `开启`   |

## Input

![Input 图标](img/input.jpg "Input 图标")

This section is about input peripherals.

### Mouse

|                    名称                     |                                               用途                                                |   类别   |         默认值         |
| ------------------------------------------- | ------------------------------------------------------------------------------------------------- | -------- | ---------------------- |
| `Sensitivity`                               | Adjust the sensitivity of the mouse cursor. If changed it may automatically enable `Raw Input`.   | 滑条     | `1x`                   |
| `Raw Input`                                 | Read mouse/tablet positional values directly from the hardware，without any post-processing.      | Button   | 关闭                   |
| `Map absolute raw input to the osu! window` | Confine input devices with absolute positioning (e.g. pen tablets) to the osu!客户端 window only. | Button   | 开启                   |
| `Confine mouse cursor`                      | Prevent mouse cursor from leaving the osu!客户端 window. See below for details.                   | 下拉菜单 | `Only when fullscreen` |
| `Disable mouse wheel in play mode`          | Disable mouse wheel during gameplay. Using the mouse wheel can change the master volume value.    | Button   | 关闭                   |
| `Disable mouse buttons in play mode`        | Disable mouse buttons during gameplay. This is helpful for keyboard users.                        | Button   | 关闭                   |
| `Cursor ripples`                            | Show subtle ripple effect when the mouse is clicked.                                              | Button   | 关闭                   |

- When `Raw Input` is enabled，it will display the number of reports it receives per second and the latency in milliseconds.
- The cursor ripple effect can be triggered by pressing `M1` and `M2` during game play.

---

If you open the dropdown list for `Confine mouse cursor`，you will be presented with these options:

|          名称          |                                                   用途                                                   |
| ---------------------- | -------------------------------------------------------------------------------------------------------- |
| `Never`                | Never prevent the mouse from leaving the osu!客户端.                                                     |
| `Only when fullscreen` | Only prevent the mouse from leaving the osu!客户端 when fullscreen. (This also includes `Letterboxing`). |
| `Always`               | Always prevent the mouse from leaving the osu!客户端 in any resolution.                                  |

### Keyboard

|            名称            |                                                      用途                                                      |  类别  |
| -------------------------- | -------------------------------------------------------------------------------------------------------------- | ------ |
| `Change keyboard bindings` | Displays a dialog of the keyboard bindings. See [Keyboard Bindings](/wiki/Keyboard_Bindings) for more details. | Button |
| `osu!mania layout`         | Displays a dialog of osu!mania key bindings. See [osu!mania layout](/wiki/osu!mania_Layout) for more details.  | Button |

### Other

|              名称              |                                                       用途                                                       |  类别  | 默认值 |
| ------------------------------ | ---------------------------------------------------------------------------------------------------------------- | ------ | ------ |
| `OS TabletPC support`          | Improves compatibility with graphic tablets and tablet PCs.                                                      | 复选框 | `关闭` |
| `Wiimote/TaTaCon Drum support` | Enable support for Nintendo's Wii Taiko Drum controller and Wiimotes. Pair device via Bluetooth before enabling. | 复选框 | `关闭` |

## Editor

![Editor 图标](img/editor.jpg "Editor 图标")

This section is about the [beatmap editor](/wiki/Beatmap_Editor/).

These options only affect while working inside the beatmap editor or in test mode (test playing a beatmap).

### General

|           名称            |                                    用途                                     |  类别  | 默认值 |
| ------------------------- | --------------------------------------------------------------------------- | ------ | ------ |
| `Background Video`        | Play the beatmap's background video while editing.                          | 复选框 | `关闭` |
| `Always use default skin` | Use osu!'s default skin while editing，despite the current skin's settings. | 复选框 | `关闭` |
| `Snaking sliders`         | Enable snaking sliders while editing.                                       | 复选框 | `开启` |
| `Hit animations`          | Enable hit animations while editing.                                        | 复选框 | `关闭` |
| `Follow points`           | Enable follow points while editing.                                         | 复选框 | `开启` |
| `Stacking`                | Stack the hit circles as if in gameplay.                                    | 复选框 | `开启` |

These options can be manually overwritten by using the `View` menu in the beatmap editor.

## Online

![Online 图标](img/online.jpg "Online 图标")

This section is about chat，spectators，multi，and osu!direct.

### Alerts and Privacy

|                           名称                           |                                                                   用途                                                                   |  类别  | 默认值 |
| -------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- | ------ | ------ |
| `Chat ticker`                                            | Display the most recent chat message at the bottom of the screen. The message that displays is from the current channel you are viewing. | 复选框 | `关闭` |
| `Automatically hide chat during gameplay`                | If chat is open during breaks or in-game menus，the osu!客户端 will automatically hide it when gameplay starts again.                    | 复选框 | `开启` |
| `Show a notification pop-up when someone says your name` | When someone mentions your username in chat，a flashing notification will appear.                                                        | 复选框 | `开启` |
| `Play a sound when someone says your name`               | When someone mentions your username in chat，a sound will play.                                                                          | 复选框 | `开启` |
| `Share your city location with others`                   | Share your city location in your user card (your country is already shared).                                                             | 复选框 | `关闭` |
| `Show spectators`                                        | Show a list of current spectators on the left of the screen during gameplay.                                                             | 复选框 | `开启` |
| `Automatically link beatmaps to spectators`              | Send currently-playing beatmap to `#spectator` channel when you have spectators.                                                         | 复选框 | `开启` |
| `Show notification popups instantly during gameplay`     | Allow a push notification to display during gameplay. If disabled，osu!客户端 will wait until you are done playing.                      | 复选框 | `开启` |
| `Allow multiplayer game invites from all users`          | Allow multi game invites from anyone. Disabling this will limit multiplayer invites to friends only.                                     | 复选框 | `开启` |

### Integration

|                    名称                    |                                                               用途                                                               |  类别  | 默认值 |
| ------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------- | ------ | ------ |
| `Integrate with Yahoo! status display`     | Your Yahoo! messenger will show the song you are currently playing or listening to. Needs to be set from the osu!website.        | 复选框 | `关闭` |
| `Integrate with MSN Live status display`   | Your Windows Live Messenger will show the song you are currently playing or listening to.  Needs to be set from the osu!website. | 复选框 | `关闭` |
| `Automatically start osu!direct downloads` | (For [osu!supporters](/wiki/osu!supporter/) only) When spectating or multiplaying，the beatmap will be downloaded automatically. | 复选框 | `开启` |
| `Prefer no-video downloads`                | (For [osu!supporters](/wiki/osu!supporter/) only) osu!direct downloads will be confined to no-video versions of beatmaps.        | 复选框 | `关闭` |

### In-Game Chat

|                     名称                      |                         用途                          |  类别  |  默认值   |
| --------------------------------------------- | ----------------------------------------------------- | ------ | --------- |
| `Filter offensive words`                      | Replace offensive words with `*beep*`.                | Button | `关闭`    |
| `Filter foreign characters`                   | Removes any non-standard ASCII characters.            | Button | `关闭`    |
| `Log private messages`                        | Private messages will be saved to the `osu!/` folder. | Button | `关闭`    |
| `Block private messages from non-friends`     | Enabling this will confine PMs to friends only.       | Button | `关闭`    |
| `Chat ignore list (space-separated list)`     | Words you put here will be ignored.                   | Text   | _(Empty)_ |
| `Chat highlight words (space-separated list)` | Words you put here will be highlighted in chat.       | Text   | _(Empty)_ |

## Maintenance

![Manitenance 图标](img/manitenance.jpg "Manitenance 图标")

This section is about beatmaps，updates，and debugging (cuttingedge only).

### General

|            名称             |                                                          用途                                                          |  类别  |
| --------------------------- | ---------------------------------------------------------------------------------------------------------------------- | ------ |
| `Delete all unranked maps`  | Delete all unranked maps in your songs folder.                                                                         | Button |
| `Repair folder permissions` | Give read/write permission to the osu!客户端 for access to its folders. (Will need administrator password to proceed.) | Button |
| `Mark all maps as played`   | Mark all maps as "played".                                                                                             | Button |
| `Run osu! updater`          | Close the osu!客户端 and open the updater to search for updates and download if any.                                   | Button |

### Debug

These settings are only in cuttingedge.

*Caution：Restarting the osu!客户端 does not revert these settings and that enabling `Debug_DisableSpriteDraw` will make the screen black (you may have trouble trying to turn this back off)!*

|               名称                |                    用途                     |  类别  | 默认值 |
| --------------------------------- | ------------------------------------------- | ------ | ------ |
| `Debug_NoAsyncReads`              |                                             | 复选框 | `关闭` |
| `Debug_DisableGCLowLatency`       |                                             | 复选框 | `关闭` |
| `Debug_DisableBackgroundSaves`    |                                             | 复选框 | `关闭` |
| `Debug_DisableTextRendering`      | Stops updating and rendering text.          | 复选框 | `关闭` |
| `Debug_DisableSpriteDraw`         | Stops drawing everything.                   | 复选框 | `关闭` |
| `Debug_DisableBlendingModes`      | Set every sprites' blend mode to Normal.    | 复选框 | `关闭` |
| `Debug_DisablePerformanceLogging` | Stops saving performance issues in the log. | 复选框 | `关闭` |
| `Debug_DisableTextureUploads`     | Stops updating certain sprites and text.    | 复选框 | `关闭` |
| `Debug_ForceIPv4FallbackPath`     | Force use of IPv4 instead of IPv6.          | 复选框 | `关闭` |
| `Debug_DisableBancho`             | Completely disables osu!bancho.             | 复选框 | `关闭` |
| `Debug_DisableFBO`                |                                             | 复选框 | `关闭` |
| `Debug_DisableVBO`                |                                             | 复选框 | `关闭` |
| `Debug_DisableMultipleVBOs`       |                                             | 复选框 | `关闭` |
| `Debug_DisableSliderRendering`    | Stops _all_ sliders from being rendered.    | 复选框 | `关闭` |

### Build Version

Last but not least，the osu!客户端 build version.

Here，you can see which build version you currently have and which type of build updates you are receiving.
Clicking on this will direct you to the Release Notes using your preferred browser.

The builds are versioned using this scheme:

```
b{YYYY}{MM}{DD}.{revision}{type}
```

- `{YYYY}` is the build year
- `{MM}` is the build month
- `{DD}` is the build day
- `{revision}` is the build revision
  - If there is no build revision number，the decimal point will be removed.
- `{type}` is the build type
  - If there is no build type value，assume it is `Stable`.

## Trivia

- If you type in a name but leave the password form empty，_osu!_ will use that name when saving the score locally.
- Opening the options sidebar will automatically trigger `osu! is up-to-date!`'s function (check for updates).
- The `Seasonal backgrounds` option was added after positive feedback was given to the osu!team.
  - More details：[main menu background changes](https://osu.ppy.sh/community/forums/topics/606931)

### History

- The old options screen was an actual screen that had tabs，buttons，and a dark pale blue background.
- The old options screen also featured a skin selection screen that also allows you to preview live play of a beatmap in osu!standard.
  - After the options screen was moved over to a sidebar，this screen was still accessible by opening a skin file.
    - Access to this was later removed after Skin Previews and the Live Preview functions came to be.
