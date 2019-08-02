<!-- wiki -->
[Game_Modes wikilink]: ../ "游戏模式页面"
[Play_Styles#osu!catch wikilink]: /wiki/Play_Styles/ "更多信息可以在玩法风格页面下的 osu!catch 一节找到"
[Score#osu!catchSV wikilink]: /wiki/Score/#osu-catch "评分部分的介绍可以在 Score 文章的 osu!catch 得分值部分找到"
[Options#Keyboard wikilink]: /wiki/Options/ "更多信息可以在设置中的键盘部分找到"
[Skinning#osu!catch wikilink]: /wiki/Skinning/osu!catch/ "osu!catch 皮肤制作"
[Mascots#Yuzu wikilink]: /wiki/Mascots/#yuzu "更多信息可以在吉祥物页面（英文）里的 Yuzu 部分找到"
[Auto wikilink]: /wiki/Game_Modifiers "更多信息可以在游戏 Mod 页面里的 Auto 部分找到"
[Hidden wikilink]: /wiki/Game_Modifiers "更多信息可以在游戏 Mod 页面里的 Hidden 部分找到"
[Flashlight wikilink]: /wiki/Game_Modifiers "更多信息可以在游戏 Mod 页面里的 FlashLight 部分找到"
[Relax wikilink]: /wiki/Game_Modifiers "更多信息可以在游戏 Mod 页面里的 Relax 部分找到"
[osu! wikilink]: /wiki/Game_Modes/osu!/ "osu!"

<!-- external -->
[ouendan wikipedia]: https://en.wikipedia.org/wiki/Osu!_Tatakae!_Ouendan "维基百科中的「押忍！战斗！应援团」页面"

<!-- image -->
[osu!catch logo]: /wiki/shared/CtB_logo.jpg "特殊模式下的 Catch the Beat 图标"

<!-- shared image -->
[osu!catch icon link]: /wiki/shared/mode/catch.png "osu!catch 图标"
[osu!catch Playfield]: /wiki/shared/Catch_Playfield_27.jpg "osu!catch 游戏区域大小的差异"
[Fruits image]: /wiki/shared/Catch_fruits.jpg "osu!catch 中的水果"
[Fruit trails image]: /wiki/shared/Catch_trails.jpg "osu!catch 中的水果轨迹"
[Bananas image]: /wiki/shared/Catch_bananas.jpg "osu!catch 中的香蕉雨"
[Hyperfruit image]: /wiki/shared/Catch_hyperfruits.jpg "osu!catch 中的超级水果"
[osu!catch Interface image]: /wiki/shared/Interface_ctb.jpg "osu!catch 的界面"
[Options keyboard image]: /wiki/shared/Options_keyboard.jpg "设置中的输入图标，键盘一节"

<!-- Title -->

# osu!catch

**[点击返回到「游戏模式」页面][Game_Modes wikilink]**

<!-- Uncomment the below and delete this comment if ScoreV2 is official and the whole page must be revised to fit ScoreV2 system behaviour -->
<!-- **[Click here to visit the older version of osu!catch using deprecated ScoreV1 system](./v1 "osu!catch v1")** -->

![Gameplay of osu!catch][osu!catch Interface image]

osu!catch, 以前叫做 _Catch the Beat_ 或 _CtB_。这个游戏模式需要玩家控制游戏中的角色（接果人），让它能及时接住循节奏从上面掉下来的水果。 

## ![osu!catch icon][osu!catch icon link] 游玩

### 谱面选择界面

要进入 osu!catch 模式，请同时按下 `Ctrl` + `3` 。

或者，点击左下角的 `Mode` 然后选择 `osu!catch`.

### 游玩基础

#### 游戏区域

![osu!catch 游戏区域大小在 CS2 与 CS7 之间的差异][osu!catch Playfield]

_图中左边是 CS 为 2 时的游戏区域大小，右边是 CS 值为 7 时的游戏区域大小。_

游戏区域的缩放大小取决于谱面设定的 CS（即缩圈大小）值。CS 值越低，游戏区域的缩放程度就越大，角色的移动空间就会越窄。反之亦然，CS 值越高就意味着游戏区域缩放程度更小、角色的移动空间越宽。

接果人可以在屏幕底部左右移动，水果要从屏幕顶部逐渐掉落。
但是接果人不能从屏幕右侧穿越到屏幕左侧。

所有接到的水果在当前的连击中断前都会一直盛在盘内。连击中断后，盘内的水果就会弹出盘外。
接水果的时机和掉在盘中的位置不会造成影响，两种情况下都可以判定为满分或 Miss 。

#### 水果（Fruits）

![水果][Fruits image]

_水果就是 osu!catch 里的打击圆圈，它们从屏幕顶部逐渐落下。_

要接到这些水果，确保水果正中水果盘，而不是掉在盘边上或者掉在盘外。
每接到一个水果就会计 300 分并将连击数 +1 ，判定为结算界面中的 300 。

#### 水果轨迹（ Fruit Trails ）

![水果轨迹][Fruit trails image]

_水果轨迹就是 osu!catch 中的滑条。_

普遍情况下水果轨迹包含两个水果（处于轨迹起始和结束）、水滴（ Droplets -- 滑条路径）、果汁液滴（Juice Drops -- 滑条白点）。如果有反向路径，就会有更多水果来充当滑条的反向箭头；水果轨迹就会按照相反方向掉落。
接到水滴会记 10 分，判定为结算页中的 50 。
接到果汁液滴会计 30 分并将连击数加 1，判定为结算页的 100 。

如果 Miss 了水果液滴（Juice Drops）就会重置连击数（因为它相当于滑条白点），而水滴（Droplets）就不会。
然而 Miss 的水滴（Droplets）尽管不会显示在游戏的结算页中，但会显示在谱面页面的排行榜的 _Miss Droplet_ 上。很明显，它还会影响你的准确度（每 Miss 一个就相当于少一个 50 判定）和总分数（每 Miss 一个就会少计 10 分）。

#### 香蕉雨（Bananas）

![香蕉雨][Bananas image]

_香蕉雨就是 osu!catch 中的转盘。_

此时香蕉们会像下雨一样掉落，并随着掉落逐渐缩小到盘子大小。
每接到一个香蕉就会加 1,100 分，Mod 和分数倍化器不影响该分数。  
它并不会减少血条，因此你可以忽略这场~~可以白嫖的~~香蕉雨。
但收集香蕉可以增加额外的分数，并且可以帮你恢复血条。
值得注意的是，[Auto][Auto wikilink] Mod 可以超越极限将香蕉全部收集，无任何遗漏。

#### 超级水果

![超级水果和接果人接到前一个超级水果后激活的冲刺效果][Hyperfruit image]

_左图：接果人接到超级水果之前；右图：接果人冲刺到水果前并留下残影_

超级水果非常特殊，它可以帮助接果人在时间跨度非常严苛、平常的移动速度无法接到的情况下接到接下来的水果。
超级水果有一个特征，它的周围有一圈明显的红色。

接到超级水果后，接果人的移动速度就会升级为 _冲刺速度_ （仅仅够接到下一个水果），颜色变成红色，并且还会在接到水果的地方留下暂时的红色残影，到接到（或者错失）下一个水果之后，接果人就会恢复正常。

## 玩法风格

**[参考《玩法风格》文章的 osu!catch 一节。][Play_Styles#osu!catch wikilink]**

## 控制

![设置中的键盘选项][Options keyboard image]

_[转到 设置 - 输入选项 中的 键盘设置，点击尽管更改按键绑定” 按钮来更改相应的按键。][Options#Keyboard wikilink]_

### 控制接果人

- 默认情况下，按左方向键 `<-` 和右方向键 `->` 移动接果人。
- 按住 `左 Shift`（或者 D ）和方向键可以让接果人以更快的 2 倍速度 _冲_ 到指定方向（此时接果人会变得更加明亮）。 
  - 你也可以按住鼠标左键来激活它。

普通模式下游戏中的光标不会控制接果人左右移动。
但如果激活了 [Relax][Relax wikilink] Mod ，你就可以用光标来控制接果人了。
不过此时你的成绩不会被上传，因为这种控制方法让 osu!catch 的唯一挑战变得毫无意义（固定的移动速度和接果盘的控制方式）。

## 评分

_[评分部分的介绍可以在 Score 文章的 osu!catch 得分值部分查阅][Score#osu!catchSV wikilink]_

评分一节详细介绍了评分系统的所有细节，包括数学公式。

### 等级

等级 | 条件
:---:|:---
SS | 100.00% 准确度
S  | 98.01% 到 99.99% 准确度（像 _osu!mania_ 一样，即使有几个 Miss 还是可以达到 S 等级）
A  | 94.01% 到 98.00% 准确度
B  | 90.01% 到 94.00% 准确度
C  | 85.01% 到 90.00% 准确度
D  | 85.00% 及以下准确度

你可以使用 _[Hidden][Hidden wikilink]_ 和 / 或 _[Flashlight][Flashlight wikilink]_ Mod 来获得银 S / SS 。

### 准确度判定

准确度由接到的水果的多少决定。香蕉雨不会影响准确度。
换句话说：`准确度 = 接到的水果总数 / 总水果数`

名称 | 公式
:---:|:---
**接到的水果总数** | 水滴数 + 果汁液滴（Juice Drops）数 + 水果数
**总水果数**        | Miss 的水果数 + Miss 的水滴（Droplets）数 + 水滴数 + 果汁液滴（Juice Drops）数 + 水果数

**例外情况：**

- 注意，香蕉（或者叫做转盘水果）作为可获得的额外奖励，并不会影响你的准确度。
还有一点，如果使用 osu!API 计算准确度，水滴（ Droplets ）的判定计数会被计算在 **`count50`** 一项中；Miss 的水滴数会被计在 **`countkatu`** 一项。

### 分数

分数计算规则和 [osu!standard][osu! wikilink] 中的分数倍化规则是一样的
但是和 osu!standard 不一样的是，水果的得分会不同于 osu!standard 。

- 普通水果的得分是 300 乘以分数倍化系数。
- 水果液滴（ Juice drops，滑条白点）计 100 分，不使用分数倍化器计算。
- 最小的液滴（ Droplet，滑条路径 ）计 10 分，不使用分数倍化器计算。
- 每个香蕉（即转盘的水果）得 1,100 分，Mod 和分数倍化器同样不影响计分。

osu!catch 中，连击不会因为 Miss 了水滴（ Droplets，在谱面分数排行榜被计为 _Miss Droplet_ ）而被打断，但通过接住水滴可以获得更高的精确度和分数。

`分数 = 打击分数 + (打击分数 * ((连击系数 * 难度系数 * Mod 系数) / 25))`

|     名称     |                        含义                         |
|:------------:|:----------------------------------------------------|
| **判定分数** | 打击圈的判定（50，100或300），滑条白点和转盘奖励分  |
| **连击系数** | (这个音符前的连击数 - 1）或者 0；取两者中更高的一个 |
| **难度系数** | 谱面的难度 (见下一节)                               |
| **Mod 系数** | 所选 Mod 的系数                                     |

**注意：** osu!standard 和 osu!catch 的分数计算方法有一些差别：There is a difference between osu!standard and osu!catch's scoring methods:-

- 完成的转盘不会计 300 分，也不会增加连击计数。
- 反向箭头处的水果会像接到普通的水果一样计分。
  - 注意，反向箭头在 osu!standard 只计 30 分。

### 打击物件的判定

**除香蕉外的所有物件**

- 接到水果等，得满分。
- Miss ，得零分。

**香蕉**

- 每接到一个香蕉就会得 1,100 分（分值固定）。
- 如果 Miss 了香蕉，不会影响任何判定。

### 分数 / 连击倍化器

**以下情况可以使分数 / 连击倍化器的系数增加：**

- 收集到水果。
- 收集到果汁液滴（ Juice drops ）。

**以下情况可以使分数 / 连击倍化器的系数重置为零：**

- Miss 了任何一个水果。
- Miss 了任何一个果汁液滴（ Juice Drops ）。

**以下情况不会影响分数 / 连击倍化器：**

- 收集到小水滴（ Droplets ）。
- 收集到香蕉。Yuzu

## 血条

用于计算血量增Yuzu
这一切都围绕着 HP 难度设置展开，只能由作图者自己设定。

**以下情况会恢复一点血量：**

- 收集到任何水果、果汁液滴（ Juice Drops ）、香蕉。

**以下情况可以导致血量减少：**

- 血量会随时间自然减少。
- 不收集任何水果和果汁液滴（ Juice Drops ）。

**以下情况不会导致血量增加或减少：**

- 休息时段。

## 皮肤

**[更多信息请参考皮肤页面下的 osu!catch 一节。][Skinning#osu!catch wikilink]**

## 作图

### osu!standard 的转谱

- 打击物件的水平坐标决定水果（滑条水果、水滴、果汁液滴）的位置。
- 打击物件的现身取决于使该物件消失的时间设定。
- 水果轨迹通过的速度和 osu!standard 上滑条球移动的速度一致。
- 转盘可以生成香蕉雨。

**注意：** 超级水果由游戏自动生成。

## 杂项

### 游戏

- [Auto][Auto wikilink] Mod _总会_ 收集全部的香蕉。
- 如果分数计使用的是 `打击偏差` 模式，osu!catch 将一直使用 `色块模式`。
- 在休息时段，玩家可以任意地移动游戏角色。
- 和 osu!taiko 模式中的 pippidon 相似，接果人也有一个 Miss 动画。
- 第一版的接果人是一个 Q 版的一本木龍太（ Ryuuta Ippongi ，来自 [应援团系列][ouendan wikipedia]）。在 2014 年以前它一直是默认的接水果角色，之后它被现在的接水果角色 [吉祥物 Yuzu][Mascots#Yuzu wikilink] 替代。
- 如果使用了 [Auto][Auto wikilink] Mod，玩家的名字就会变成 _salad!_（~~水果~~沙拉）。

### 游戏的历史

[第一个 osu!catch 谱面的链接]:https://osu.ppy.sh/s/13676 "Yousei Teikoku - Dare so Ka no Gekka (TV Size) (NatsumeRin)，带有由 Uran 制作的 osu!catch 谱面"

![特别模式的 osu!catch 图标][osu!catch logo]

_已废弃的特别模式下的 osu!catch (Catch the Beat) 图标_

- 在 2012 年 4 月 10 日前，osu!catch 谱面不能被 Ranked 或出现在 Ranked 的谱面集中。
  现在情况已经完全改变 ，只要玩家遵守作图规范，就可以针对 osu!catch 的难度进行作图。
  尽管现在 osu!catch 的作图规范还在完善当中，但随着更多 Ranked 的 osu!catch 谱面出现，以及玩家对其所给予的反馈，osu!catch 的作图规范会慢慢向 osu!standard 靠拢，更加全面和广泛。
- 第一个包含至少一个 osu!catch 的谱面是 [Yousei Teikoku - Dare so Ka no Gekka (TV Size) (NatsumeRin)，带有 Uran 制作的 osu!catch 谱面][第一个 osu!catch 谱面的链接]
- 第一个仅包含 osu!catch 谱面的谱面集是 [Rita - Hajimari no Toki (Deif)](https://osu.ppy.sh/s/91485 "Rita - Hajimari no Toki (Deif)") 。
