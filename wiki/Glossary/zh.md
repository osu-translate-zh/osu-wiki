# 专有名词表

多年来，osu!社区 采用了自己的一套术语，这些术语可能会使一些新人感到困惑。本页面是对一些术语的汇编，仅供参考。欢迎所有人添加或者编辑本页面。

## A

### 废弃的荒地（ Abandoned Wasteland ）

如果你不能理解这个名词，下面则解释了它的意思：`Abandoned Wasteland` 是一个隐藏的子论坛，关于这个子论坛的说明是：“把我们真正不需要的东西放在这里。” 当一篇帖子是或被称为无用的时候，那么这篇帖子则会被移动到这个子论坛。

### 准确率（ Accuracy ）

一个用于衡量玩家节奏的准确性的 [度量标准](/wiki/Accuracy) 。有时也被缩写成 _Acc_ 。

### 玩家长时间离开（ AFK ）

AFK 是一个网络缩写词，它的意思是 _Away From Keyboard（离开键盘或玩家长时间离开）_。举个例子，当一个活动的玩家在他还在登录的时候离开去做别的事情时，_osu!_ 将会把他的状态标记为 AFK 。

### 缩圈（ Approach Circle ）

在 [osu!standard](/wiki/osu!standard) 中，缩圈是物件最外部的圆，它将逐渐缩小直到包围要被点击的物件。缩圈也是滑条头或是转盘的中心（对于旧皮肤而言），你应该在当缩圈接近打击圈或滑条时点击。对于旧皮肤的转盘来说，缩圈则是表示转盘的旋转持续时间。

### Authentic

authentic 意思是一张谱面在特定的阶段从方方面面（歌曲、设置、物件摆放布局 等）都模仿 [DS 游戏](/wiki/DS_games) 。

### Aspire

Aspire 是一个制作谱面的 [竞赛](/wiki/contest) ，它鼓励创作者完全忽略 [Rank 标准](/wiki/Ranking_Criteria)。从本比赛中产生的谱面往往是在外观上吸引着玩家，但对普通玩家来说，这些谱面是根本无法正常游玩的。

## B

### Bancho

_相关： [BanchoBot](/wiki/BanchoBot)_

Bancho 是由 peppy 编写的一个易于扩展的服务器。在 osu! 所有需要在线管理的内容中，Bancho 代替了第三方 [IRC](/wiki/IRC)（互联网在线聊天）服务器的需求。 用 osu!账号 在游戏内登录，游戏将会自动重连直到成功连接至 Bancho 。

### 节拍（ Beat ）

节拍（ Beat ）是一个在编辑模式中应用在时间轴上的术语。歌铺可以根据它们的 BPM 为每个节拍划分出一段时间。一个正确对准节拍的谱面将使每个节拍对应于该歌曲的节奏，并且整个歌曲的节拍应该落在 [时间轴](/wiki/Timeline) 上的两条白线之间。

若想知道有关时间线的更多信息，请参阅 [音符时值](/wiki/Beat_Snap_Divisor) 。

### 节拍间距（ Beat Spacing ）

节拍间距是一个适用于 [osu!standard](/wiki/osu!standard) 模式的原则。这说明每个 [打击物件](/wiki/hit_object)（转盘除外）的间距应参照如下原则：如果物件被紧密的摆放在时间轴上，它们在谱面上的距离应该靠近一些；如果物件在时间轴上的空距较大，它们在谱面上的距离则应远一些。

![节拍间距的基础和例子](img/Beatspacing-zh.jpg "拍距的基本原理。")

这条原则基本上意味着：

- 物件的间隔的时间越近，物件在谱面上的距离就越近
- 物件的间隔的时间越远，物件在谱面上的距离就越远

当某个玩家在打你的谱面的时侯，你的节拍间距就扮演着一个十分重要的角色。一致的节拍间距是 rank 一张谱面的基本要求，因为这为玩家提供了更直观的体验，玩家将以歌曲的速度学习移动光标的位置。

如果将一个物件放在比节拍间距更近的地方，可能会让玩家过早地点击它们。另一方面，将物件放的远一些可能会让玩家在屏幕上及时移动光标以点击它们。一个常见的节拍间距的例外是堆叠打击物件。

为了保证一致的节拍间距，可以打开编辑器右边的 `Distance Snap` 按钮。你可以按住 `Alt` 键并在右上方的滑动选择器不断调整物件间的节拍间距。注意，该值越高可以使谱面更难。

### 谱面 ID （ BeatmapID ）

谱面 ID 是一个唯一的、递增的整数，它被用来标记每张上传的谱面集合的所有难度。

你可以用这个 URL 来找到某张谱面中的某个难度： `osu.ppy.sh/b/{BeatmapID}`

这个值可以在 URL 中通过改变谱面的难度选项卡找到。你可以使用游戏内的选项 `1. Beatmap Listing/Scores` 访问谱面的 URL 来找到谱面 ID ，也可以在某个谱面难度的文件 `.osu` 中找到谱面 ID 。

所有未发布的谱面的谱面 ID 则将为 `0`。

### 谱面集合（ BeatmapSet ）

谱面集合是打包在同一个 `.osz` 文件中谱面的一个集合。这些谱面集合中的谱面是由同一个作者创建的。

谱面集合中的每张谱面总是会包含相同的音乐、音效（如果制作了的话）以及视频或 Storyboard （如果有的话）。但是，请注意，某些谱面集合中的谱面可能会包含一些其它的音效、背景或 Storyboard ，这些谱面与其他的不同。

### 谱面集合 ID （ BeatmapSetID ）

谱面集合 ID 是一个唯一的、递增的整数，它被用来标记每张上传的谱面集合。

你可以用这个 URL 来找到某个谱面集合： `osu.ppy.sh/s/{BeatmapSetID}`

这个值可以在 osu!网站 中的谱面搜索列表结果中的 URL 上找到，也可以在 `Songs` 文件夹中某张谱面的文件夹名称上找到（文件夹名的第一穿数字），还可以打开谱面集合中某个难度的 `.osu` 文件查找到。

所有未发布的谱面集合的谱面集合 ID 则将为 `-1`。

### 比特率（ Bit Rate ）

几乎每个音乐文件都包含一个叫做“比特率”的东西。比特率是指一个音乐文件每秒可以通过数字网络传输的比特数。

那将意味着 *更高的比特率* 通常有着 *更高的音乐质量* （但文件大小会更大）。反之亦然，*较低的比特率* 通常有着 *较低的音乐质量* （但文件大小会更小）。

比特率通常在 96 KBps （千比特每秒）到 320 KBps 之间。这是音乐可以使用的比特率的一个相当广泛的范围。但是，[Rank 标准](/wiki/Ranking_Criteria) 明确指出了所有的音乐文件的比特率范围应该在 **128 KBps - 192 KBps** 之间。

你通常可以通过检查该文件的文件属性来检查音乐文件的比特率。另一种检查方法检查 [AiMod](/wiki/AiMod) 是否说音频文件的比特率太大。如果两种方法似乎都是对的的，这意味着你将不得不降低比特率。在 [音频编辑](/wiki/Audio_Editing) 中可以找到几种重新编码音频的方法。

### 背景（ BG ）

BG 是 _background （背景）_ 的简称。BG 是指谱面的背景图像及背景视频。在谱面文件夹中，BG （有时也叫 _bg_ ）通常是背景图像的名称。

### 覆盖（ Blanket ）

一个制谱术语，用来描述一个滑条覆盖住另一个对象的状态。 在 [这里](/wiki/Mapping_Techniques/Making_Good_Sliders#Beat-Blankets) 可以找到制作它们的指南。 

### 谱面管理成员（ BN ）

 BN 是 _Beatmap Nominator （谱面管理成员）_ 的简称，他们是 [谱面管理组](/wiki/people/Beatmap_Nomination_Group) 的成员。

### 每分钟节拍数（ BPM ）

BPM 是 _Beats Per Minute （每分钟节拍数）_ 的简称，表示一分钟内所有节拍的数量。

较高 BPM 的音乐可能与较高的 [缩圈速度](/wiki/approach_rate) 相关联，反之亦然。

### 休息时间（ Break ）

休息时间是指谱面的某段时间内没有任何的打击物件。在这段时间内，玩家将暂时不会掉血。休息时间通常允许玩家在短时间内进行休息他们的手臂并重新调整他们的输入设备。

根据设置的不同，当在休息时间时，黑边（顶部和底部的黑色横条）可能会出现在屏幕上。除此之外，如果有着足够的休息时间，则会出现通过或失败的图像以及播放声音来指示玩家上一段的成绩是否良好。

在 [osu!mania](/wiki/osu!mania) 的谱面中增加休息时间是非常不推荐的。

### 谱面提交系统（ BSS ）

BSS 是 _Beatmap Submission System （谱面提交系统）_ 的简称。

当一位 [作者](/wiki/creator) 把他们的 [谱面集合](/wiki/beatmapset) 制作完后，并准备在世界各地分享他们的成果时，他们必须使用 BSS 提交谱面。当他们这样做的时侯，BSS 将会自动分配以及生成一个帖子，其中包含关于你的谱面集合的信息。BSS 生成的论坛主题可以帮助你从修改者与其他玩你谱面的玩家那里得到一些反馈。最后，你的谱面将会被分别赋予 [谱面 ID](/wiki/beatmapid) 以及一个 [谱面集合 ID](/wiki/beatmapsetid) 。

有关完整的介绍，请查看 [提交](/wiki/Submission) 页面。

## C

### Changelog

The changelog is a page where peppy and the osu!dev team details their day-by-day improvements, additions and bug fixes.

To see the changelog, see [Recent Releases](https://osu.ppy.sh/p/changelog).

### Choke

A choke occurs when the player almosts obtains a full combo while playing a beatmap, but combobreaks near the end.

On the contrary, a reverse choke is when the player combobreaks at the beginning but obtains a full combo for the rest of the beatmap.

### Collab

Collab (short for _collaboration_) has two meanings:

1. the work of multiple [creators](/wiki/creators) [beatmapping](/wiki/beatmapping) a single [beatmap](/wiki/beatmap); usually a [marathon](/wiki/marathon) beatmap
   - When collaborating on a beatmap, the creator must map a majority (at least half) of the beatmap. This is to ensure that the creator has done enough to upload the map under their username.
2. the mapset containing [guest difficulties](/wiki/guest_difficulty)

Collab may sometimes be used in [difficulty](/wiki/difficulty) version names.

### Combo

Combo has two meanings:

1. a set of hit circles and sliders that comes one after another (also called a _comboset_)
2. the number representing the number of objects a player has hit consecutively without missing or [sliderbreaking](/wiki/sliderbreak) once
   - this number is displayed in various places:
     - bottom-left in [osu!standard](/wiki/osu!standard)
     - on the drums in [osu!taiko](/wiki/osu!taiko)
     - above the fruit catcher in [osu!catch](/wiki/osu!catch)
     - centre of the stage in [osu!mania](/wiki/osu!mania) (vertical height varies by skin)

A _max combo_ is simply the player's highest achieved combo throughout the play.

### Combo Colour

The combo colour is a colour that that separates a comboset from another.

In osu!standard, all [combosets](/wiki/comboset) have a colour. A new combo is started when the colour of the hit object changes. The colours will keep repeating themselves depending on how many the mapper defined (or how many your skin's `skin.ini` file defines). There is a minimum of 2 and a maximum of 8 combo colours.

In osu!catch, each fruit is coloured in the order given. Droplets and end-slider fruit will always have the same colour as the start-fruit. However, bananas will always have a tint of yellow.

When editing a beatmap, one can change those colours and/or their order in the [Song Setup](/wiki/Song_Setup) section.

For skins, the skin properties for the combo colours is located on in the `[Colours]` section of the `skin.ini`. However, do note that the skin's defined combo colours is only used when the mapper does **not** define them.

### Combo Fire

![Ancient screenshot of the combo fire](/wiki/shared/combo-fire.jpg "R.I.P. combo fire")

The combo fire was a background gameplay feature from the ouendan game integrated in _osu!_ This would display a burning yellow flame after obtaining the first [combo milestone](/wiki/combo_milestone), 30. If the player obtains a combo of 500, the combo fire colour will change from yellow to blue. The combo fire will extinguish itself if the combo was broken but would still be reobtainable.

This feature was later disabled on 05. March 2013 due to performance concerns.

### Combo Milestone

A combo milestone is a set of numbers that will shoot stars and display a comboburst (if enabled in the [options](/wiki/options)) after obtaining one of these milestones.

The combo milestones for osu!standard and osu!catch are 30, 60, 100, and multiples of 50 after 100. For osu!taiko, the combo milestones are multiples of 50. For osu!mania, the combo milestones are multiples of 100.

### Combo Multiplier Effect

The combo multiplier effect occurs in the osu!standard, osu!taiko, and osu!catch game modes. This occurs because said game modes use the player's current combo as a part of the score calculations. Meaning that a player would get a higher score, if they had gotten a full combo, than someone who played the same map with a broken combo.

However, if you obtain a combo of ~10,000, your score will begin to count backwards. This is a flaw with the 32-bit signed integer where (in computing) the max integer is 2,147,483,647. A fix, [scoreV2](/wiki/scorev2), for this is still being tested.

### Combobreak

A combobreak is when the player loses their combo during any part of playing a beatmap.

### Comboburst

A comboburst is a celebration of achieving a [combo milestone](/wiki/combo_milestone).

- For osu!standard and osu!catch, a character will _burst_ out from either the left or right side of the window
- For osu!taiko, a collection of flowers will _burst_ behind pippidon
- For osu!mania, a character will _burst_ from the right side of the stage (or left side if specified in the `skin.ini`)

In addition to this, for osu!standard, osu!taiko, and osu!catch, stars will shoot out from either the left or right side of the playfield, for combos less than 100, then both sides for combos 100 or higher. For osu!mania, the starts will shoot out from the stage.

Combobursts can be disabled in the options.

### Comboset

A comboset is a group of combos that starts their count at 1 and goes up for each hit circle and/or slider until a slider or a new comboset starts.

The last object in a comboset can help give the player a little health boost if they obtain a hit score of 300.

In osu!catch, once a comboset is completed, the fruit will jump off of the plate.

### Cookie

![Screenshot of main menu](img/Intro_static.jpg "The cookie is typically used to describe the circular osu!logo which appears at the very start of the game, and refers to its shape.")

The cookie is another word for the _osu!_ logo. This has appeared many times in the osu!client. The cookie is seen in the main menu, in solo mode, and previously in old crash reports as seen below.

![Window dialog of osu! crashing](img/Pippi_corruption.jpg "Pippi! Get that cookie out of your mouth - it could be dirty...")

### Creator

A creator refers to the user who uses the [beatmap editor](/wiki/beatmap_editor) to create a [beatmap](/wiki/beatmap).

## D

### Difficulty Stars

The difficulty stars is the visual representation of a beatmap's [difficulty](/wiki/difficulty) version. This rating is (theoretically) between 0 and 10 stars based off of an algorithm.

_osu!_ currently uses two different algorithms to calculate difficulty stars:

- peppy's algorithm
  - determined by using the bonus difficulty score multiplier and eyup's algorithm (use the difficulty tags are assigned)
- Echo's algorithm (not in use)

You can see a beatmap's difficulty when testing it in the editor. The difficulty stars can be seen on the song selection screen or at its listing in the site.

### Downbeat

Downbeat is a musical term for the first beat of a measure.

This term was coined from orchestral conducting because when the baton moves in a downward motion, it depicts the first beat of the measure.

### Drain Time

The drain time, or _drain_, refers to the total duration of the beatmap that requires the player to be active. Drain time does not consider the breaks and unmapped parts throughout the beatmap.

Maps with very long drain times are typically referred to as [marathon](/wiki/marathon) maps and require endurance beyond the norm in order to complete successfully.

Maps must have at least 45 seconds of drain time be considered rankable.

### Drop and Droplet

A Drop is an osu!catch element that gives a score of 100, equivalent to slider ticks in osu!standard, while Droplets give a score of 10, equivalent to the slider track in osu!standard.

Missing a Drop breaks the player's combo, but missing a Droplet does not.

The visual difference between Drops and Droplets is that a Drop is twice as big as Droplets are.

### DS

DS is an abbreviation meaning _distance snapping_. This term is usually seen during the modding process.

### DS Games

DS games is a collective term for _[Osu! Tatakae! Ouendan!](https://en.wikipedia.org/wiki/Osu!_Tatakae!_Ouendan)_ (also called "Ouendan" or "Ouendan 1"), _[Moero! Nekketsu Rhythm Damashii Osu! Tatakae! Ouendan! 2](https://en.wikipedia.org/wiki/Moero!_Nekketsu_Rhythm_Damashii_Osu!_Tatakae!_Ouendan!_2)_ (almost always called "Ouendan 2") and _[Elite Beat Agents](https://en.wikipedia.org/wiki/Elite_Beat_Agents)_ (also called "EBA").

A set of rhythm games, developed by [iNiS](https://en.wikipedia.org/wiki/INiS) for the Nintendo DS handheld video game system, which share a lot of gameplay and presentation elements.

The osu!standard game mode was is mostly based off of those games.

## E

### EBA

EBA has two meanings:

- Elite Beat Agents, one of the DS games that _osu!_ is based on.
  See [Elite Beat Agents - Wikipedia](https://en.wikipedia.org/wiki/Elite_Beat_Agents) for more details.
- The collective term for the playable characters in that game (referring to meaning above) (e.g. "The EBA" or "The Agents").

## F

### Fail

Fail has three meanings:

- the incompletion of a beatmap due to:
  - not filling the healthbar up to 80% when completing a beatmap (in [osu!taiko](/wiki/osu!taiko))
  - empty healthbar ([osu!standard](/wiki/osu!standard), [osu!catch](/wiki/osu!catch), and [osu!mania](/wiki/osu!mania))
- in multiplayer, an indicator underneath the player's name to show they have failed the beatmap
- the player having less than 50% health during a break; where an indicator will display if you failed the section
  - a fail indicator will be shown
  - a failed storyboard animation will be played instead (if available).

### FC

![Score comparison between full and broken combos](img/CombosCanHurt.png "The score on the top has a full combo, while the one on the bottom has a broken combo.")

FC, short for _full combo_, is when a player completes a beatmap while obtaining the maximum combo possible. This does not account accuracy as it is often used to mean clearing a beatmap without having any misses or [sliderbreaks](/wiki/sliderbreak).

Due to the [combo multiplier effect](/wiki/combo_multiplier_effect), full combos will give the most score in the osu!standard, osu!taiko, and osu!catch modes.

## G

### Geki

Geki(激), or _Elite Beat!_, is a scoring term used when you complete a [comboset](/wiki/comboset) with the highest accuracy on every note.

### Grade

A grade, usually confused with "rank", is a letter-grade that represents the player's performance after playing a beatmap. It accompanies the total score at the result screen and appears in all lists where scores appear.

From lowest to highest, the possible grades are D, C, B, A, S, Silver S, SS, and Silver SS.

### Graveyard

A subforum for beatmaps that were abandoned. Graveyarded maps do not count towards a user's total upload limit. The owner may revive them on their profile, which sends them back to being a Work in Progress. This requires having a free pending slot.

Beatmaps that are not updated or receive no posts from their owner for 28 days will be automatically sent to the Graveyard.

### Grid Snapping

Grid snapping refers to a button on the right hand side of the editor screen.

Enabling it will force every newly placed (or existing, but moved) object to snap along the intersections of the grid.

The base level of spacing between each sector of the grid can be adjusted by pressing `G` or by going to `View` then `Grid Level`. Grid snapping can help with aligning objects to each other and arranging them in patterns.

### Guest Difficulty

Guest difficulty, or _GD_, refers to any difficulty made by a mapper for inclusion in another mapper's set. Guest difficulties usually have the mapper's username as the difficulty's name.

There are many reasons for guest difficulties to exist:

- etiquette in the community can make it difficult for multiple creators to upload beatmaps of the same song around the same time
  - a different mapper, interested in mapping that song, may choose to contribute a difficulty to the other mapper's set instead
- they may also decide, after-the-fact, upon playing the other map that they like the music and want to create a difficulty for it
- or the mapper does not want to put in the effort in creating the difficulties on their own, but rather would want to just create one and give it to another mapper

On the other hand, it may be the creator who wants a few guest difficulties:

- to give the mapset a "community effort" feel
- simply because they do not want to create such difficulties by themselves

Guest difficulties are often requested by private messages in-game or via forum private messages. Guest difficulties can also be requested in the modding queues, especially those who are offering to do them.

More than one guest mapper is allowed to contribute to a beatmapset, including creators from any one of the four game modes. If an additional game mode is to be featured in a mapset, that game mode must have at least two difficulties that follows the [Ranking Criteria](/wiki/Ranking_Criteria). Each guest creator is also allowed to create more than one difficulty to contribute to the mapset, as long as the number of difficulty versions created by the guest mapper does not exceed the number of difficulty versions of the creator/uploader (this is to determine who should upload the mapset).

## H

### Hit Sound

Hit sounds are the sounds that _osu!_ plays in response to user input when completing one of the hit objects in the game. This is in contrast to the underlying music and sounds created by the user interface.

Hit sounds are used to provide an auditory feedback mechanism to the player to help them judge their timing. These are complementary to approach circles and spacing which are the visual mechanisms used to communicate timing information.

There are 4 types of hit sounds:

- _(normal)_ (used when none of the below are used)
- whistle
- clap
- finish

These are added to make the hit sounds sound more expressive and let the player feel more like they are part of the music. _osu!_ provides a wide array of hit sounds (eight in the stable release, since upgraded to twelve). Though, creators can go further add up to 24 more. Sliders also have ambient sound effects when they are being performed successfully, including a recurrent ticking sound which matches the beat.

## I

### Ignore List

The ignore list is a blacklist of words (or users) that the player does not want to be displayed in the [chat console](/wiki/chat_console).

## K

### Katu

Katu(喝), or _Beat!_, is when you complete a particular combo without achieving the highest level of accuracy throughout that set.

This is different than a Geki(激) because the comboset was not done perfectly with 300s.

### Keys

In [osu!mania](/wiki/osu!mania), the number of keys can determine the map's difficulty. The more keys you have, the more the player has to focus for each key column.

### Kiai

Kiai is a term given for a "special" timing section to help emphasize a part of a beatmap. A player can tell if a part of a beatmap has a kiai timing section by seeing added visual effects such as flashing beats, flying stars, and fountains.

Keep in mind that overuse and abuse of kiai can be disorienting! Thus [creators](/wiki/creators) are advised to use it judiciously (or when it makes sense).

### Kudosu

![Kudosu Durp](img/Kudosu-Durp.png "Kudosu Durp")

Kudosu is a form of reward obtained from modding beatmaps. The term "Kudosu" is named after a combination of the words "kudos" and "osu!".

A rating system that rewards users that mod regularly. If you are a [BN](/wiki/BN), or the creator of the map, you can award 1 or 2 kudosu to a user depending on the time since last post on the beatmap thread, making a constructive modding post. Accumulated kudosu can be used to increase a beatmap's priority rating. Any mapper or modder may spend 1 kudosu to give any map a star, which will help the map in the approval process by giving it more star priority.

Before awarding kudosu keep the following things in mind:

- Did the post help you in any way **to improve your map**?
- Did the modder post things **that AIMod cannot pick up**?
- Did the post show that the modder has **knowledge of modding**?
- Did the modder post things that generally **make sense to you and seem not too terribly picky?** If their post did seem picky, are you sure that the things pointed out **can improve your mapset anyways?**
- Even if you do **not** follow the modder's advice, did you not follow it because of **your personal choice only**, and not because **the modding seemed pointless to you?**
- Did you not already give the modder kudosu for a mod post on the same map **recently**, and if you did, has the map **vitally changed** between the two mod posts (adding a difficulty, remapping a difficulty)?
- Was this a **substantial mod post?** Did the mod post point out more than a couple of things to improve or fix your map?

If you can answer yes to all of these questions, **feel free to give the modder their well-earned kudosu!**

![](img/Givekudosu.jpg "Button to give a Kudosu!")

The creators of a beatmap can give a modder kudosu by simply going to the mod post and click the `Give Kudos` button that is located under the poster's information. Please be aware that beatmap nominators may revoke your kudosu if they deem that your post should not have been awarded kudosu!

## L

### Lead-in

The lead-in time is a 3 second time period of silence that is sometimes automatically be inserted before the beginning of a beatmap.
This only happens if the creator has placed objects right at or very close at the start of the song.

### Life Bar

The life bar, also known as the _health bar_, _HP bar_, _spirit bar_, or _ki bar_, is a bar at the top left of the playing screen for [osu!standard](/wiki/osu!standard), [osu!catch](/wiki/osu!catch), and [osu!taiko](/wiki/osu!taiko). For [osu!mania](/wiki/osu!mania), the life bar is rotated 90 degrees anti-clockwise and is placed next to the bottom-right of the stage.

In all modes, expect for osu!mania, there is a symbol moving along it indicating the player's life. If the bar is completely empty, the player fails the current beatmap (assuming no special game modifiers are enabled).

osu!standard and osu!catch will have health drain at a constant rate throughout the course of a beatmap, except during breaks.

For osu!standard, the bar is replenished by the player [tapping](/wiki/tap) hit circles, following sliders and slider ticks, and spinning spinners. The more accurate the tapping, the bigger the boost. The player also receives larger boosts if he achieves a [katu](/wiki/katu) or an [geki](/wiki/geki) at the end of a combo.

For osu!catch, this can be done by catching fruit and drops.

For all game modes (expect osu!taiko), a sizeable part of the bar is also depleted in case of a miss.

### Local Song Offset

The local song offset is an offset set for individual [beatmaps](/wiki/beatmaps), not the entire beatmapset itself. This is to offset the beatmap's offset alongside the global offset.

You can change your local song offset by pressing:

- `+` to increase the offset by 5 milliseconds
- `-` to decrease the offset by 5 milliseconds
- `Alt` + `+` to increase the offset by 1 milliseconds
- `Alt` + `-` to decrease the offset by 1 milliseconds

If you play a beatmap that has a local song offset, _osu!_ will tell you that there the previous offset will be used.

### Loved

A state of ranking for beatmaps that don't follow the [ranking criteria](/wiki/Ranking_Criteria) and are therefore unrankable, but are considered popular enough to deserve their own leaderboards. Loved beatmaps contribute to a user's total playcount, but does not contribute to their performance points.

### Looping

From the [ranking criteria](/wiki/Ranking_Criteria), the required [drain time](/wiki/drain_time) **must** be at least 30 seconds. If your audio clip is shorter than that, you *should* loop it.

## M

### M4M

M4M, or _Mod for Mod_, is a term describing when a modder agrees to mod another modder's map in return for a mod on their own map.

### Marathon

A marathon is a type of [beatmap](/wiki/beatmap) that can only be approved.

Marathon beatmaps are considered to be at least 6 minutes long and can only have one mapped difficulty. However, some marathon mapsets may contain a single [osu!taiko](/wiki/osu!taiko) variant as well.

Marathon beatmaps are often collaborative efforts, as mapping longer tracks is a draining endeavour when done solo.

Upon the creation of the marathon beatmap, one should name their beatmap version "Marathon" to bypass the [BSS](/wiki/bss) from preventing the pending status.

### MAT

**As of the 23. April 2013, all members of the MAT at that time were promoted as full members of the [BAT](/wiki/BAT), with the MAT team decommissioned.**

The MAT, meaning _Modding Assistance Team_, was a group of users experienced in modding. MAT members were able to mark any beatmap they approve of with a bubble. This bubble would note that the beatmap as worthy of further consideration by the BAT.

### Mod Request

A mod request is when a mapper is in need of help.
This can be from fixing possible mistakes to requesting for [guest difficulties](#guest-difficulty).
While, typically, the song is still playable, the only reason someone would scroll here is if (and only if) you know what you are (and will be) doing and willing to mod the map for them.

Keep in mind that the map or mapset may be incomplete, so be a considerate person and (if you had tried the map) tell them what is wrong with the mapper's map.

### Modder

A modder is a term given to a user that gives comments or suggestions on another [mapper's](/wiki/mapper) [maps](/wiki/maps) in the [forums](/wiki/forums). Doing so is called [_modding_](/wiki/modding), and the posts are referred to as _mods_.

Activities are shown either at [Works In Progress/Help](https://osu.ppy.sh/forum/10) (including the [Modding Queues](https://osu.ppy.sh/forum/60)) and/or [Pending Beatmaps](https://osu.ppy.sh/forum/6).

## N

### NC

NC has two meanings:

1. short for _new combo_, a modding term to suggest that a beat needs to be the start of a new combo
2. an abbreviation for the [Nightcore mod](/wiki/Nightcore), a variant of the [Double Time](/wiki/Double_Time) mod that increases the pitch of the music and adds a consistent bass drum beat to the music.

### NM

NM has two meanings:

1. short of _NoMod_, used to describe when a player does not enable any [game modifiers](/wiki/Game_Modifiers).
2. an abbreviation for Normal, used as [difficulty](/wiki/Difficulties) name for [osu!mania](/wiki/Game_Modes/osu!mania) beatmaps.

### Nuke

Any [beatmap](/wiki/beatmap) that is considered to be disregarding the rules (or the mapper disregarding the [Code of Conduct](/wiki/Modding_and_Mapping)) can be nuked. Nuked beatmaps are considered "closed" until significant changes are made and the status is manually removed by a member of the team.

Examples include but are not limited to:

- not following the basics of the guidelines
  - containing really bad timing
  - has objects placed randomly on the grid and/or timeline but are also extremely challenging or unconventional beatmaps (e.g. consisting of a single spinner).

The warning icon that accompanies nuked beatmaps is the symbol for radioactive materials (![radioactive icon](/wiki/shared/icon/nuke.gif)).

## O

### Offset

The offset is a period of time between the beginning of a beatmap's song file and the instant the first beat of the rhythm is heard, from which the position of the first beat is calculated. This is measured in milliseconds (ms).

The offset is the first half of beatmap timing, where the other half is the [BPM](/wiki/bpm).

### Online Song Offset

The online song offset is an offset that is **already** applied to a beatmap after it was ranked.

Adjusting your [local song offset](/wiki/local-song-offset) will only add more to this value.

### osu!

_osu!_ has three meanings:

- The rhythm video game for the Microsoft Windows Operating Systems.
  Spelled with a lowercase "o" and an exclamation mark at the end.
- The game mode (unofficially called _osu!standard_ to prevent ambiguity).
- An informal greeting in the Japanese language, resulting from condensing the phrase "Ohayo gozaimasu!" (Good morning!)
  - Pronounced with a silent u ("OSS").
  - Close English equivalents include "Yo!" or "Hey!".
    To read more about its meaning in Japanese language and culture, see [Does anyone here speak/learn Japanese?](https://osu.ppy.sh/forum/p/2686).

### osu!coin

- osu!academy introduces the osu!coins: [Introduction to osu!coins](https://www.youtube.com/watch?v=BImc5McuK1o)
- peppy announces the osu!coins: [osu!coins!](https://osu.ppy.sh/home/news/2015-03-31-osucoins)

The osu!coin was the in-game currency that was still "in development", as a 2015 April Fools joke.

After peppy realizes that the current rate of return would not allow him to purchase a private jet within his lifetime, the osu!coin was introduced as the new in-game currency. Every player will start off with 10 osu!coins and will be given 10 osu!coins per day. Existing users will get an additional two osu!coins right off the bat.

One osu!coin will give the player one play, while retrying a beatmap will consume one osu!coin. If the player obtains a combo that is a multiple of 100, they will obtain one osu!coin. If the player runs out of osu!coins, they may purchase more—out of their own will—with these exchange rates:

- 1USD = 1 osu!coin
- 10USD = 10 osu!coins
- 999USD = 1000 osu!coins (0.001% savings!)
- first unborn child = infinite osu!coins (unborn child will work for osu!)

The following day, peppy rolled back the implementation of osu!coins due to popular demand, and ended with [this remark](https://disq.us/p/w2ydos).

### osupixel

An osupixel is the representation of one screen pixel when _osu!_ is running in 640x480 resolution. osupixels are one of the main coordinate systems used in osu!, and apply to hit circle placement and storyboard screen coordinates (these pixels are scaled over a 4:3 ratio to fit your screen).

In contrast, textures are scaled such that one texture pixel ([texel](https://en.wikipedia.org/wiki/Texel_%28graphics%29)) corresponds to one screen pixel at 1024x768 resolution.

### Ouendan

Ouendan has three meanings:

- In Japanese culture, a cheer squad which, similar to western cheerleaders, rallies a sports team on using drums, horns, banners and yells of encouragement.
- The pair of Japanese DS games that _osu!_ is based on.
  This term may sometimes be used to refer specifically to the first of these games.
- A collective term for the playable characters in the aforementioned games, e.g. "The Ouendan".

### Overmapping

Overmapping is when the hit objects or placement of hit objects are placed in a way that makes the difficulty of the map contrast the actual song.

This can be done by adding unnecessary jumps, slider speed-ups, or by mapping to an unknown beat in the music consistently (ie. adding notes on blue ticks when the song is only using red ticks), in order to add difficulty.

There are two ways to avoid this:

1. Jumps, slider speed-ups, and other difficulty increasing techniques should only be used when they fit with the music.
   - If there is no sudden change that requires (or could greatly be supplemented with) then simply do not add them.
   - Insane beatmaps are not to show how hard you can make a beatmap, but rather how well you can make a map that is difficult but fun.
2. The map might not need an Insane difficulty.
   - If you feel that your map is too boring without adding a plethora of difficulty increasing techniques, then maybe your map does not need it.
   - Remember, mapsets do not require a Insane difficulty, so you will be just fine without one.

This topic was discussed in an episode of [osu!talk](/wiki/osu!talk) ([osu!talk special Over Mapping](https://www.youtube.com/watch?v=RepSYE3hN3A)) that overmapping actually has a positive effect in [osu!taiko](/wiki/osu!taiko) maps because the drums plays an important role in a song.

## P

### Pass

Pass has two meanings:

- the completion of a [beatmap](/wiki/beatmap) with or without the use of mods
- the player having more than 50% health during a [break](/wiki/break)
  - an indicator will display if you passed the section

### peppy

peppy, written with a lowercase `p`, is the online alias of Dean Herbert.
He is the creator of the _osu!_ project and its primary developer.

### Play Time

Play time is the total duration of a beatmap.
This includes the lead-in time and the break time(s).

### pp

Short for [_performance points_](/wiki/Performance_Points). The main ranking metric of the game.

### puush

puush is a screen capturing and file uploading application developed by peppy.
puush is a successor of sorts to upppy which is commonly used to upload and share images in _osu!_

For more information about puush, see [puush / home](https://puush.me).

## Q

### QAT

Short for [_Quality Assurance Team_](/wiki/People/Quality_Assurance_Team). Used to refer to the group itself or one of its members.

## R

### Rank

Rank has three meanings:

1. another word for a letter grade
2. a player's standing in the online leaderboard (a.k.a. player ranking)
3. the verb "to rank", which is when someone second another moderator's nomination and include a submitted beatmap to the ranked beatmap list, making scores achieved by anyone playing it count towards each player's ranking.
   Getting their beatmaps ranked is usually the goal of creators.

### Ranking

Ranking, alternatively called _leaderboard_, is a list that sorts members of the osu!community according to certain criteria. This can also refer to one's position in such a list.

_osu!_ currently has five rankings:

- [PP](/wiki/pp) rankings: the ranking most commonly referred to, based on the player's pp.
- Chart rankings: based on ranked score for beatmaps in a chart.
- Score rankings: based on the player's ranked score.
- Country rankings: based on the collective scores of player's per country.
- [Kudosu](/wiki/kudosu) rankings: based on the user's kudosu! count.

### Recalc

Recalc is short for _Recalculate slider lengths_. Recalc is a command under the `Timing` header of the editor screen.

Usage of this is suggested after a [BPM](/wiki/bpm) change is made, if the beatmap already has sliders. This command will automatically adjust the length of every slider in the beatmap to the new BPM. If used, it is important, especially if a large change in BPM has been made, to check every slider and adjust its length manually, where necessary.

### Resnap

Resnap is a pair of commands under the `Timing` header of the [editor](/wiki/editor) screen. One of which applies to the entire [beatmap](/wiki/beatmap) and the other to the current timing section (if the beatmap has only one timing section, both commands are the same).

Usage is suggested when there has been a change in offset and/or BPM, after objects have been placed. This command will automatically reposition all objects on the timeline so that they fall on the closest beat division your snap divisor allows. If used, it is important, especially if a large change in BPM and/or offset has been made, to check every object and adjust its position on the [timeline](/wiki/timeline) manually, where necessary.

### Restricted Mode

Restricted mode is a state automatically applied to accounts that are suspected to breaking the [TOS](/legal/terms). Submitted scores of gameplay are not allowed publically displayed.

For more info, see [What is "restricted" mode, exactly?](/wiki/Help_Center#what-is-"restricted"-mode,-exactly?).

### RSI

RSI, short for _Repetitive Strain Injury_, is a type of injury that affects the musculoskeletal and nervous system of the body. This can be caused by doing repetitive tasks in an awkward position which may include playing _osu!_ for an extended amount of time.

## S

### Sample Set

A sample set is the collection of sound effects that are heard during gameplay.

These are categorized under three names:

- Normal
- Soft
- Drum

Inside each categories has these four hit sounds:

- _(normal)_ (the sound when none of the below is used)
- whistle
- clap
- final

However, there are other parts of a sample set that may include the slider tick sounds and the sound made when filling the spinner metre.

### Silence

A silence is an action taken against an user who spams the [chat console](/wiki/chat_console). Silences will stack on top of each other, adding more time for each one.

Silences lasts for 4 weeks before being reset, along with the time that gets added.

### Skin

A skin is a set of graphics and custom sample sets (audio clips) that can replace the default ones used by osu! This will allow for a more customised user experience. Most of what you see and hear in _osu!_ can be skinned.

To see the dedicated sub-forum for skins, see [Skinning](https://osu.ppy.sh/forum/15).

To see the list of skinnable elements, see [Skinning](/wiki/Skinning) (and its subpages).

### Skinner

A skinner refers to the user who releases downloadable skins in the [forums](/wiki/forums).

### Sliderbreak

Sliderbreak has two meanings:

- In [osu!standard](/wiki/osu!standard):
  - tapping the slider-start too early (this can cause the slider to shake)
  - not collecting a slider tick (includes the hidden ones underneath the slider-start and slider-end)
  - releasing the slider ball before it hits the slider-end
    - this will not cause a miss, rather it will give you a 100 with no combo increment
- The case where the player does not obtain the max possible combo without missing an object.

### Slider Tick

The slider tick is a hit object that gives out 10 points. The amount of slider ticks used in a slider is dependent on the slider velocity, the [BPM](/wiki/bpm) and the inherited timing.

### Spectate

Spectate, or spec, is when someone watches another player playing a [beatmap](/wiki/beatmap) in real time (with approx. 500ms delay).
To spectate, open the extended chat and click on a grey user panel.

For this to work, you will need to have a copy of the exact same beatmap the player you wish to spectate is playing. However, if you have an [osu!supporter](/wiki/osu!supporter) tag, the beatmapset will be downloaded and loaded for you.

### Spectator Aura

Spectator aura is a mysterious phenomenon that could cause players to [choke](/wiki/choke) their [combo](/wiki/combo), or fail a beatmap from having a spectator(s) spectate their gameplay.

### Stacked

Stacked objects are hit objects that overlap each other in the playfield. The most common object that is stacked are hit circles.

Stacking hit circles (a clear violation of beat spacing) is, nevertheless, permitted if the hit circles are very close to each other in the timeline (half a beat or usually even less).

### Standard

_See also: [osu!](/wiki/Game_Modes/osu!) (game mode)._

Standard refers to the game mode in _osu!_ and has been used since it is the first game mode. This is sometimes stylized as _osu!standard_ or osu! (without italics).

This term is used greatly within the osu!wiki to prevent ambiguity between _osu!_ (the framework, game client, etc.) and the game mode itself.

### Star

Star has four meanings:

1. A stage in a beatmap's modding process where a moderator judges a beatmap to be on the right track but needing some improvements before approve with a bubble.
   - Examples include adjustments in timing, incorrect beat spacing in some areas, or creating additional difficulty versions.
   - Beatmaps receiving a star are denoted by a star graphic next to their thread's title.
   - A star may be removed by another mod if the beatmap is thought to be in need of more improvements.
2. another term for "Difficulty Stars"
   - The symbol that represents the difficulty of a beatmap.
3. another term for "[Kudosu](/wiki/kudosu)"
   - These are given to beatmap modders and can be used to raise a beatmap above others.
4. another term for "[Star Priority](/wiki/star_priority)"
   - These stars are given to [osu!supporters](/wiki/osu!support) and are used in [Feature Requests](https://osu.ppy.sh/community/forums/4).

### Star Priority

Star priority has two meanings:

1. Star priority is a method of helping Beatmap Nominators to find beatmaps worthy of bubbling and later ranking.
   - The star priority of a beatmap is determined by how many mod posts that have gained kudosu in the beatmap's thread, the sum of kudosu stars the map set has received.
   - A kudosu star can be given by any user to any map, though shooting a kudosu star comes at the price of one kudosu.
   - The conversion rate was formerly three kudosu for one kudosu star that increased the Star Priority by two.
   - The higher the star priority, the higher the beatmap's thread appears in the Works in Progress or Pending subforum.
   - At least 12 star priority is needed for a map to be bubbled or ranked.
2. A method in determining whether a Feature Request is wanted by the community.
   - The higher the star priority, the faster it gets noticed.
   - Users that have supporter status active when voting will shoot a pink star (![Kudosu](/wiki/shared/Kudos.png)) that increases Star Priority by 2 each, whilst a user without supporter will shoot a blue star (![Star](/wiki/shared/icon/star.gif)) that is worth only 1 each. Users may be able to shoot multiple stars depending on how many votes they have left.

### Storyboarder

A storyboarder refers to the user who makes storyboards for their own or someone else's [beatmap](/wiki/beatmap). They may have used the editor's design section to [storyboard](/wiki/storyboard), used a third party application, or have done [storyboard scripting](/wiki/storyboard_scripting) (or SBS).

### SV

SV, meaning _slider velocity_, is the speed in which the slider moves at in relation to the BPM. This term may sometimes be used during the modding process.

The slider velocity defines the movement speed of the slider ball. The lower the slider velocity, the slower the slider ball.

## T

### Tablet

A graphics tablet is an alternative input medium to the computer mouse.

A tablet consists of a flat surface on which one can point and/or drag using an attached stylus, if one is included. The image of the screen does not appear on the tablet, thus making it different in functionality from a touch screen.

### TAG

A TAG difficulty is a type of beatmap that is designed for more than one person to play at the same time in [multiplayer](/wiki/multiplayer) mode, using the Tag Coop/Tag Team Vs Team Mode.

Each player is responsible for one comboset, where each hit object in that comboset is mapped to be extremely farther apart, making it nearly impossible to play by a single player. Therefore it becomes a challenge for elite players in terms of precision of jumping.

TAG difficulties are usually named TAG in a beatmap set. TAG2 maps are meant for 2 players, while TAG4 maps (the hardest) are meant for 4 players.

Note that TAG difficulties are unrankable because they are intentionally not designed for a single player. However, this has not stop users from trying.

### Tap

In [osu!standard](/wiki/osu!standard), tapping is a term that means "to press a button while the cursor is over a hit object". Tapping hit objects at the right moment, as indicated by the beatmap's music and the approach circle, is an essential part of _osu!_ gameplay. There are a few different buttons one can use to tap:

- the left and right mouse buttons,
- the `Z` and `X` keys on the keyboard,
- using the buttons on the tablet/touchpad, or
- directly on a touchscreen/tablet

### Test Mode

Test mode is a feature of the [beatmap editor](/wiki/beatmap_editor). This allows you to test your beatmap without having to submit anything. However, you are required to save the beatmap before continuing to test mode; creating issues if you need to rollback on your recent changes.

### Time Signature

The time signature is a musical term that indicates how many beats are in each measure and what note value constitutes a single beat. _osu!_ offers two alternative time signatures, which can be selected from the Timing menu: 4/4, which is the one most commonly used, and 3/4, which is selected when the rhythm of the song is of, or similar to, a waltz.

### Timing Section

Good timing of a beatmap is big a requirement for a beatmap to get ranked. Timing a beatmap consists of determining the offset and then the BPM of the song it uses.

When the tempo changes, you are required to add a new timing section to accompany the new tempo.

The timing process creates the timeline on which objects will be placed.

One of many reasons as to why your timing of a beatmap is important because _osu!_ takes the given [BPM](/wiki/bpm) and offset to determine where the hit objects should go. If your timing is off, even by a little, then it is next to unrankable to map hit objects on the editor.

### Touchpad

A touchpad is a substitute for the computer mouse. Touchpads are most commonly found on laptop computers. The touchpad usually consists of a small rectangular area which one can drag one's finger to move the mouse cursor. Due to the way touchpads are designed, they do not work with a stylus or similar devices.

### Touchscreen

A touchscreen is one of the input mediums used by the DS games that _osu!_ is based on. _osu!_ supports touchscreen functionality, but the hardware required is generally expensive for the average player. A computer whose entire screen functions as a touchscreen is called a Tablet PC. This is different than a tablet because a touchscreen has some kind of display while tablets do not.

### Touhosu!

_Feature Request forum thread: [Touhosu!](https://osu.ppy.sh/forum/t/19307)_

Touhosu! is a requested game mode that is the opposite of osu!catch. _Opposite_ because instead of catching objects, you avoid them.

The name _Touhosu!_ is a combination of _Touhou_ (the shoot 'em up/bullet hell games) and _osu!_.

## U

### Universal Offset

The universal offset is the time delay between:

- the object graphics and sample set sounds associated with them
- the point of the song where they should be heard

The universal offset applies to all songs used in _osu!_ and its value differs according to each system's specifications. After being determined, it does not need to be modified again. An incorrectly universal offset will cause timing problems in every beatmap played or edited. If everything sounds off to you while playing a few ranked [beatmaps](/wiki/beatmaps), try checking your universal offset. The universal offset settings is located in the [Options](/wiki/Options).

### upppy

upppy is a fast and easy-to-use uploading service coded by peppy. If you want to share a file with the osu!community, forget about depositing it on Rapidshare, Megaupload, ImageShack, etc., just put it on upppy and everyone is happy! :)

For more information about upppy, see [upppy!](https://up.ppy.sh) **(NSFW: there may be a few stray images that may contain R-18 work)**.

## V

### Version

Version has four meanings:

- the specific [beatmap](/wiki/beatmap) of the [beatmapset](/wiki/beatmapset)
  - this term can be used in place of beatmap to prevent disambiguation
  - they could be called "Easy", "Normal", "Hard", "Insane", or "Expert"
  - however, creators are allowed to give custom names to the difficulty versions of their beatmaps
- the version of a skin
  - see [Skinning](/wiki/Skinning) for more details
- the release date of your osu!client
- the build release of your osu!client (Stable, Stable (Fallback), Beta, and cuttingedge)

## W

### WIP

WIP is an acronym for _Work In Progress_.

There are various reasons to mark a beatmap as WIP:

- deemed incomplete by its creator
- incomplete difficulty versions
- only one difficulty versions or not enough difficulty versions
- pending correction
- suggestions on the timing
- needs feedback

WIP can be submitted through the [BSS](/wiki/bss) to the Beatmap Help [forum](/wiki/forum) to get comments, feedback, and help from mods and other users.

## Z

### z/x

z/x are the default keys on the keyboard to [tap](/wiki/tap) in _osu!_ A very popular alternative to the left and right mouse buttons.

During gameplay, while `Z` is pressed, the left mouse button will not work and vice versa. The same applies to the `X` key and the right mouse button and vice versa.

The keyboard tapping keys can be changed in the options menu.
