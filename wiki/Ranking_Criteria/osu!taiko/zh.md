osu!taiko Ranking Criteria
==========================

_父页面：[Ranking Criteria](/wiki/Ranking_Criteria)_

这些规则和指南在 [Ranking Criteria 论坛版块](https://osu.ppy.sh/forum/87)中被讨论出来。一些正在讨论中的新规则和指南，一旦意见达成一致，将会被更新。

术语
---------

### 难度名
- ![Kantan](/wiki/shared/diff/easy-t.png "Kantan") **Kantan**: 简单 (Easy)
- ![Futsuu](/wiki/shared/diff/normal-t.png "Futsuu") **Futsuu**: 普通 (Normal)
- ![Muzukashii](/wiki/shared/diff/hard-t.png "Muzukashii") **Muzukashii**: 困难 (Hard)
- ![Oni](/wiki/shared/diff/insane-t.png "Oni") **Oni**: 恶魔 (Insane)
- ![Inner/Ura Oni](/wiki/shared/diff/expert-t.png "Inner/Ura Oni") **Ura/Inner Oni**: 里恶魔 (Expert)

更多的难度名请参考[这篇帖子](https://osu.ppy.sh/community/forums/topics/178700)。

前缀 `Inner` 或 `Ura` 可能被用于表示一个比基础难度高，但是比下一个层次的难度低的难度。（比如：Ura Kantan 比 Kantan 难，但比 Futsuu 简单点。）

### 游戏物件
- **Don / Red Note**：红圈 / 红音符，在太鼓中心击打的节拍（beat）（默认按键是 `X`，`C`）。
- **Kat / Blue Note**：蓝圈 / 蓝音符，在太鼓边缘击打的节拍（默认按键是 `Z`，`V`）。
- **Big Don / Big Red Note / Finisher Note**：大红圈 / 大红音符，在太鼓中心同时击打来获得额外分数的强节拍。
- **Big Kat / Big Blue Note / Finisher Note**：大蓝圈 / 大蓝音符，在太鼓边缘同时击打来获得额外分数的强节拍。
- **BPM**：每分钟的节奏数（beats per minutes）的缩写，用于确定一首歌的节奏速度。
- **Slider / Drumroll**：滑条 / 黄条，一个黄条中带有标记，可以击打其中的任何音符。这些标记通常是间隔 ¼ 拍（根据歌曲的 BPM 不同而不同）。如果 BPM 低于 125，标记的间隔会变成 ⅛ 拍。如果 BPM 高于 250，间隔会变成 ½ 拍。如果滑条速度（slider tick rate）被设为 3，滑条标记间隔会变成 ⅓ 拍。
- **Spinner**：转盘，一个转动的物件，要求玩家交替击打红圈和蓝圈固定的次数，次数显示在转盘的中心。敲击次数由谱面的整体难度（OD）和转盘的长度决定。
- **Bar Line**：当 BPM 高于 75 时在游戏中显示，用于判断音符的开始。如果 BPM 低于 75，将会在每一拍之间显示。
- **Overlap**：在游戏中，一个部分或者完全包含其他音符的音符。
- **Rest Moment**：一段没有音符的时间，通常用于让玩家放松双手，迎接即将到来的音符。
- **Stream**：一系列连续不断的圈。一般间隔是 ¼ 拍。
- **Snapping**：放置一个物件的时间线记号。
- **Variable Snapping**：根据歌曲本身的特点，在一小段时间内使用多种不同的组合方式来排列音符。
- **Slider Velocity**：滑条速度，Speed at which the notes/drumrolls/spinners/bar lines move horizontally from right to left through the playfield. Base slider velocity can be controlled in the timing panel and additional changes can be made through inherited (green) timing points.
- **Smooth Slider Velocity Changes**：一种从高到低或者从低到高逐渐改变滑条速度（SV）的技巧。为了达到这一效果，这些渐变的音符会有变化的滑条速度（SV）。
- **Improvisation**：拥有比歌曲实际拥有更多的音符。
- **Taiko Template Background**：模仿原版太鼓达人（Taiko no Tatsujin）的背景图片。经常包含在间歇显示的艺术家和歌曲名称的黑色信息条。

## 通用

### 规则

规则就是规则，有强制性和约束性。它们不是指南，在任何情况下都不允许被违背。

- **Each note must have its color clearly distinguishable from the previous and upcoming notes.**
- **Every note must be clearly assignable to a musical layer or layer unit it tries to represent, be it to enhance a layer the song provides, or be it an additional layer improvised by the mapper.** Do not improvise in a fashion that shifts the pace, contradicts the general music movement or misinterprets the song's current intensity. Improvising must either enhance a current layer of the song or add a new one. Otherwise, relation to the song is given up and this contradicts the main purpose of a rhythm game.
- **The `Omit first bar line` feature of an uninherited timing point must be used when a BPM change/metronome reset would hinder gameplay experience aesthetically by adding unnecessary bar lines.**
- **Taiko template backgrounds must not be used.** Due to various screen resolutions being common they do not work as they were originally intended to.
- **You must not wrongly snap sliderends to correct missing slider ticks.** This behaviour is unintended and will be corrected in the future.

### 指南

Guidelines may be violated under **exceptional** circumstances. These exceptional circumstances must be warranted by an exhaustive explanation as to why the guideline has been violated and why not violating it will interfere with the overall quality of the creation.

-   **滑条速度**

滑条速度应该是1.40或1.60 给于 Muzukashii 或以上的难度. 对于 Kantan/Futsuu, 一般使用1.00和1.20.

-   **连打**

对于大多数图来说, 1/1, 1/2和1/4的连打已经足够了. 1/3和1/6在原曲出现时可以使用. 任何情况下都请避免使用1/8.

-   **改变BPM**

物件叠在一起会让玩家感到困扰, 这个时候我们可以用绿线使速度平滑地下降. 如果不影响可读性(物件不重叠), 改变滑条速度也不是严格禁止的.

-   **黄条 (滑条)**

黃条需分开使用，而且要与其他物件有1/2拍以上的间隔。在BPM125或以下的歌不应使用黃条，因为这时黃条=1/8串。在1/3的歌曲中必须用Tick Rate 3(因为会给出1/3或1/6黃条)。

-   **风船 (转盘)**

在风船与其他物件之间至少应该有1/2拍以上的间隔。在连打中使用风船是允许的。不推荐用非常短的风船，因为他们会遮住物件，并且可能让玩家因为疯狂按键导致miss。

-   **自定义音效**

自定义音效必须是鼓类的音效. 如果使用自定义音效的话, don的音色应该比较偏低而kat音色比较比don偏高.
