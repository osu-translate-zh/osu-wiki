osu!taiko Ranking Criteria
==========================

_父页面：[Ranking Criteria](/wiki/Ranking_Criteria)_

这些规则和指南在 [Ranking Criteria 论坛版块](https://osu.ppy.sh/forum/87)中被讨论出来。一些正在讨论中的新规则和指南，将会在意见达成一致后更新。

术语
---------

### 难度名
- ![Kantan](/wiki/shared/diff/easy-t.png "Kantan") **Kantan**：简单 (Easy)
- ![Futsuu](/wiki/shared/diff/normal-t.png "Futsuu") **Futsuu**：普通 (Normal)
- ![Muzukashii](/wiki/shared/diff/hard-t.png "Muzukashii") **Muzukashii**：困难 (Hard)
- ![Oni](/wiki/shared/diff/insane-t.png "Oni") **Oni**：恶魔 (Insane)
- ![Inner/Ura Oni](/wiki/shared/diff/expert-t.png "Inner/Ura Oni") **Ura/Inner Oni**：里恶魔 (Expert)

更多的难度名请参考[这篇帖子](https://osu.ppy.sh/community/forums/topics/178700)。

前缀 `Inner` 或 `Ura` 可能被用于表示一个比基础难度高，但是比下一个层次的难度低的难度。（例如：Ura Kantan 比 Kantan 难，但比 Futsuu 简单点。）

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
- **Taiko Template Background**：模仿原版太鼓达人（Taiko no Tatsujin）的背景图片。通常包含在休息时间显示的艺术家和歌曲名称。

## 通用

### 规则

规则就是规则，有约束性和强制性。它们不是指南，在任何情况下都不允许违背规则。

- **Each note must have its color clearly distinguishable from the previous and upcoming notes.**
- **Every note must be clearly assignable to a musical layer or layer unit it tries to represent, be it to enhance a layer the song provides, or be it an additional layer improvised by the mapper.** Do not improvise in a fashion that shifts the pace, contradicts the general music movement or misinterprets the song's current intensity. Improvising must either enhance a current layer of the song or add a new one. Otherwise, relation to the song is given up and this contradicts the main purpose of a rhythm game.
- **The `Omit first bar line` feature of an uninherited timing point must be used when a BPM change/metronome reset would hinder gameplay experience aesthetically by adding unnecessary bar lines.**
- **Taiko template backgrounds must not be used.** Due to various screen resolutions being common they do not work as they were originally intended to.
- **You must not wrongly snap sliderends to correct missing slider ticks.** This behaviour is unintended and will be corrected in the future.

### 指南

Guidelines may be violated under **exceptional** circumstances. These exceptional circumstances must be warranted by an exhaustive explanation as to why the guideline has been violated and why not violating it will interfere with the overall quality of the creation.

- **Use AiMod with caution**. It is known to cause bugs related to base Slider Velocity.
- **Avoid covering essential parts of your background with the taiko playfield.** If this happens, consider altering the last zero in the `.osu` via notepad in the `0,0,"name_of_background.file_extension",0,0` line under the `[Events]` header. Positive values will lower the background while negative values will move it up.
- **If slider velocity changes are in use, they should correspond to pacing changes in the song.** That means not speeding up calm parts, or slowing down fast paced parts of a song.
- **Avoid using smooth slider velocity changes over sections which include variable snapping.** Doing so impacts the readability of these snappings, so keep the variation low enough to avoid overlapping.
- **Avoid abrupt slider velocity changes within patterns that already overlap (e.g. 1/4 streams).** Smooth slider velocity changes should be used in these cases to ensure that the patterns stay readable.
- **Substantial overlapping should be avoided so that the color of each note is still easily readable and does not pose unnecessary visual disturbance.** Overlapping should only be done if the song's pacing or note snapping at that point could justify it.
- **Avoid rhythms which are in no way predictable.** Rhythm can be made intuitive through the usage of consistent timeline gaps bridging between different snappings or through rest moments.
- **Kiai time should only be used for the chorus or emphasized parts of a song.** Kiai flashes/short kiais are discouraged for several reasons: they disturb the gameplay experience especially on low-end PC users, and can cause trouble for epileptic users.
- **The base slider velocity should be 1.40 throughout all difficulties of a mapset.** This is to ensure optimal quantity of notes on the playfield, as well as the optimal distance of separation between different notes.
- **Slider tick rate should be set according to the song.** In most cases, it should be set to 1. If the song uses 1/3 as its main snapping, use tickrate 3 to snap the drumroll ticks to 1/3.
- **Avoid following multiple layers of the song if it is unclear which rhythm is being prioritized.** Players should be able to discern what part of the song is being followed.
- **Use low volume or silent spinners only when it suits a low volume section of the song.** In most other scenarios, having audible hit sound feedback on spinners is highly recommended.
- **Songs with variable BPM may use frequent slider velocity changes in order to keep the scrolling speed at which notes move approximately constant.** Doing this will make the timeline gaps between notes easily predictable and enhance gameplay experience by avoiding overlaps due to BPM changes.
- **Avoid visually obstructing notes on the playfield with active spinners.** Spinners cover the majority of the screen, so ending them too close towards the upcoming notes can result in reading spikes. Usually having 1/2 distance between a spinner and the following note solves this.
- **There should be at least 1/2 distance between a spinner and its preceding note.** This is to ensure they do not overlap substantially and assure readability.
- **If custom hit sounds are in use, they should be drum-related.** Heavier/lower tones should be set as don and a lighter/higher tones should be set as kat.

## Difficulty-specific

**Rhythm related guidelines and rules apply to approximately 180 BPM maps.** If your song is drastically faster or slower, some variables might be different. Apply reasonable judgment in these cases.

If the beatmap follows a double or halved BPM style, Slider Velocity and all snapping variables in this ruleset need to be adjusted respectively.

### ![Kantan](/wiki/shared/diff/easy-t.png "Kantan") Kantan

#### Rules
- **If a 1/2 pattern is used, the patterns must stay simplistic and be followed by a rest moment.** For songs that follow a swing beat, this limit is 1/3.
- **Patterns on snaps faster than 1/2 are disallowed.** These patterns are too complex for beginner players. For songs which follow a swing beat, this limit is 1/3 instead.

#### Guidelines
- **1/1 patterns should not be longer than seven notes.** Anything longer is likely to be too straining for beginners. Patterns like these should be followed by a rest moment.
- **Main snapping should consist of mostly 2/1, 4/1, or slower rhythms.** Occasionally using 1/1 rhythms is acceptable.
- **Try to insert at least 1 rest moment that is 3/1 or longer after 16/1 to 20/1 of continuous mapping.** Less frequent rest moments or shorter ones may put too much strain on beginners.
- **Slider velocity changes may be used cautiously.** Changes should only happen for sections of different pacings and slider velocity should not be drastically variable.

#### Difficulty Setting Guidelines
- OD should be 4 or less.
- HP should be 6 or more. In cases of higher note count, HP could be slightly adjusted to lower than 6.

### ![Futsuu](/wiki/shared/diff/normal-t.png "Futsuu") Futsuu

#### Rules
- **Patterns on snaps faster than 1/3 are disallowed.** These patterns are too complex for beginner players.

#### Guidelines
- **1/3 patterns should not be longer than two notes.** Anything longer is very situational and usually too complex for newer players. Patterns like these should be followed by a rest moment.
- **1/2  patterns should not be longer than seven notes.** Anything longer is likely to be too straining for beginners.
- **Main snapping should consist of mostly 1/1, 2/1 or slower rhythms.** Occasionally using 1/2 rhythms is acceptable.
- **Try to insert at least 1 rest moment that is 2/1 or longer after 16/1 to 20/1 of continuous mapping.** Less frequent rest moments or shorter ones may put too much strain on beginners.
- **Simple Slider velocity changes may be used.**

If you plan on using a Futsuu as the lowest difficulty of a mapset, it has to abide by the following rules and guidelines:

#### Rules
- **Patterns on snaps faster than 1/2 are disallowed.** These patterns are too complex for beginner players.

#### Guidelines
- **1/2 patterns should not be longer than four notes.**
- **Slider velocity changes should be used cautiously.** Changes should only happen for sections of different pacings and slider velocity should not be drastically variable.

#### Difficulty Setting Guidelines
- OD should be 5 or less.
- HP should be 5 or more. In cases of higher note count, HP could be slightly adjusted to lower than 5.

### ![Muzukashii](/wiki/shared/diff/hard-t.png "Muzukashii") Muzukashii

#### Rules
- **Patterns on snaps faster than 1/6 are disallowed.** These patterns are too complex for the target audience of this difficulty level.
- **Finisher notes must not be used in any 1/4 patterns in this difficulty.** These patterns are not suitable for this difficulty level.

#### Guidelines
- **1/6 patterns should not be longer than four notes on moderate to low BPM (~140).** Anything longer is very situational and normally too complex. Patterns like this should be followed by a rest moment and avoided at faster BPMs.
- **1/4 patterns should not be longer than five notes.** Anything longer is likely to be too straining for intermediate players.
- **Main snapping should consist of mostly 1/2, 1/1 or slower rhythms.** Occasionally using 1/4 rhythms is acceptable.
- **Try to insert at least 1 rest moment that is 3/2 or longer after 16/1 to 20/1 of continuous mapping.** Less frequent rest moments or shorter ones may put too much strain on intermediate players.
- **Manipulating slider velocity is allowed**, but slider velocity should only be changed for sections of music with different pacings and should not be drastically variable.
- **1/4 patterns with one or more color changes should be used sparingly.** They should be avoided in conjunction with other patterns of this nature because the target audience of this difficulty level is not used to patterns of this complexity.
- **1/4 patterns which are longer than three notes should consist of one color change at most which should take place at the start or the end of the pattern.** Patterns more complex than that would be too demanding for intermediate players. These patterns should be followed by a rest moment.

#### Difficulty Setting Guidelines
- OD should be 5 or less
- HP should be 5 or more. In cases of higher note count, HP could be slightly adjusted to lower than 5.

### ![Oni](/wiki/shared/diff/insane-t.png "Oni") Oni

#### Rules
- **Patterns on snaps faster than 1/8 are disallowed.** These patterns are too complex for the target audience of this difficulty level.

#### Guidelines
- **1/8 patterns should not be longer than two notes.** Anything longer is very situational and normally too complex. Patterns like this should be followed by a rest moment.
- **1/4 patterns should not be longer than nine notes.** Anything longer is likely to be too straining for the target audience of this difficulty level.
- **Main snapping should consist of mostly 1/2 and occasional 1/1 rhythms.** 1/4 rhythms may be used more frequently at this level of difficulty.
- **Try to insert at least 1 rest moment which is 1/1 or longer after 16/1 to 20/1 of continuous mapping.** Longer periods of continuous mapping may put too much strain on players of this difficulty level and shorter rest moments would count as continuous mapping.
- **1/4 patterns which are longer than five notes should avoid complicated color changes.** Longer patterns with such complexity would be too demanding for the target audience of this difficulty level.

#### Difficulty Setting Guidelines
- OD should be 5 or more
- HP should be 5 or more. In cases of higher note count, HP could be slightly adjusted to lower than 5.

### ![Inner/Ura Oni](/wiki/shared/diff/expert-t.png "Inner/Ura Oni") Inner/Ura Oni

#### Guidelines
- **Main snapping should consist of mostly 1/2 and 1/4 rhythms.** 1/4 rhythms may be used very frequently at this level of difficulty.

#### Difficulty Setting Guidelines
- OD should be more than 5.
- HP should be 5 or more. In cases of higher note count, HP could be slightly adjusted to lower than 5.
