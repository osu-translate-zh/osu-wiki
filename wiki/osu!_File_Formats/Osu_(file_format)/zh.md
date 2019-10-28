# .osu (文件格式)

**.osu** 是装着对应谱面的明文文件格式。

## 总结构

其中第一行详述了这个文件的信息。例如：

`osu file format v12`

下面列出各段标题，在文件中它们被方括号标出。

例如：

`[General]`

-   General - 谱面的详细信息。
-   Editor - 作图相关的设置。
-   Metadata - 歌曲与谱面的介绍。
-   Difficulty - 直接决定歌曲难度的参数。
-   Events - storyboard的事件列表。
-   Timing Points - 谱面的时间点和音效的列表。
-   Colours - combo的RGB。
-   Hit Objects - 谱面的击打物件列表。

## General

AudioFilename (String) 描述了音频文件相对于当前文件夹的位置。

`AudioFilename: 03 artcore JINJA.mp3`

AudioLeadIn (Integer, 毫秒) 在音乐开始播放前添加的空白时间。可以给即刻播放的音乐一个准备时间。

`AudioLeadIn: 2000`

PreviewTime (Integer, 毫秒) 界定在选谱界面被选中时，音乐从什么进度播放。

`PreviewTime: 10013`

Countdown (Integer) 决定在第一个物件出现之前的倒计时的有无和速度。（0=无，1=标准，2=慢，3=快）

`Countdown: 0`

SampleSet (String) 决定使用哪组打击音效。

`SampleSet: Soft`

StackLeniency (Decimal) 决定在时间上有多相近的两个坐标相同的物件会被判定为重叠。

`StackLeniency: 0.7`

Mode (Integer) 决定这个谱面的游戏模式。（0=osu!，1=Taiko，2=Catch the Beat，3=osu!mania）

`Mode: 0`

LetterboxInBreaks (Boolean) 决定是否在休息时段显示黑边。

`LetterboxInBreaks: 0`

StoryFireInFront (Boolean) 决定是否让 Storyboard 盖住连击闪光。

`StoryFireInFront: 0`

SkinPreference (String) 决定在运行该谱面时使用哪个皮肤。

`SkinPreference:Default`

EpilepsyWarning (Boolean) 决定在开始时是否警示“This beatmap contains scenes with rapidly flashing colours..." （该谱面包含有快速闪烁的场景...）。

`EpilepsyWarning: 0`

CountdownOffset (Integer) 决定倒计时早多少节拍开始。

`CountdownOffset: 0`

WidescreenStoryboard (Boolean) 决定 Storyboard是否为宽荧屏模式。

`WidescreenStoryboard: 0`

SpecialStyle (Boolean) specifies whether or not use the special `N+1` style for osu!mania.<!--NT-->

`SpecialStyle: 0`

UseSkinSprites (Boolean) 决定 Storyboard 是否调用玩家皮肤。

例如[Algebra](https://osu.ppy.sh/beatmapsets/654033/#taiko/1386414)就调用了玩家的很多模式物件的皮肤。

`UseSkinSprites: 0`

## Editor

Bookmarks (Integer List, 毫秒) 列出了每个作图标记所在的时刻。

`Bookmarks: 94171`

DistanceSpacing (Decimal) is a multiplier for the "Distance Snap" feature.<!--NT-->

`DistanceSpacing: 1.22`

BeatDivisor (Integer) 决定对节拍的划分，作为在时间轴上摆放物件的依据。

`BeatDivisor: 4`

GridSize (Integer) specifies the size of the grid for the "Grid Snap" feature.<!--NT-->

`GridSize: 4`

TimelineZoom (Decimal) 决定时间轴的缩放程度。

`TimelineZoom: 1.5`

## Metadata

Title (String) 是用ASCII记录的曲名。

`Title:artcore JINJA`

TitleUnicode (String) 是用 Unicode 记录的曲名。如果没有，用 Title 替代这行参数。

`TitleUnicode:アートコア神社`

Artist (String) 是用ASCII记录的作曲家。

`Artist:An`

ArtistUnicode (String) 是用 Unicode 记录的作曲家。如果没有，用 Artist 替代这行参数。

`ArtistUnicode:An`

Creator (String) 记录作谱者的用户名。

`Creator:Flower`

Version (String) 记录对应谱面的难度。

`Version:Hard`

Source (String) 描述音乐的来源。

`Source:Touhou`

Tags (String List) 是对与歌曲有关的关键字的汇集。 Tags 可在osu!网站搜索栏或是选谱界面搜索栏内查找。

`Tags:niiru renka chou ~ ancients Hakurei Reimu Amamiya Yuko`

BeatmapID (Integer) 是对应谱面的ID。

`BeatmapID:297410`

BeatmapSetID (Integer) 是整套谱面集的ID。

`BeatmapSetID:114987`

## Difficulty

下列四条参数直接决定难度。0\~10星越来越难（当然，也可以超过十星）。

```
HPDrainRate:4
CircleSize:3.3
OverallDifficulty:4
ApproachRate:4.8
```

### HP Drain Rate

*HPDrainRate* (HP)决定血量掉的有多快。

HP在未来可能会改动。<!--NC需检查可能改动的是"该描述"还是"HP"--原文The definition of this property may be changed in the near future.-->

### Circle Size

*CircleSize* (CS)决定了在 osu!standard 模式中物件的半径大小。

在 osu!pixels 中，物件半径的算法为`32 * (1 - 0.7 * (CircleSize - 5) / 5)`，或是`54.4 - 4.48 * CircleSize`。

*CircleSize*的值必须在2\~7之间，否则不能 Ranked 。<!--NT原文The value of *CircleSize* for ranked beatmaps must stand at from 2 to 7, inclusive.-->

In osu!mania mode, *CircleSize* is the number of columns.<!--NT-->

### Overall Difficulty

*OverallDifficulty* (OD)决定了在时间上判定范围的宽窄、转盘至少要转多快。

- 当 OD < 5: `spins_per_second = 5 - 2 * (5 - OD) / 5`
- 当 OD = 5: `spins_per_second = 5`
- 当 OD > 5: `spins_per_second = 5 + 2.5 * (OD - 5) / 5`

下面的表格提供各得分的判定范围的具体算法：

| 得分 | 判定范围                      |
| ---- | ----------------------------- |
| 50   | `150ms + 50ms * (5 - OD) / 5` |
| 100  | `100ms + 40ms * (5 - OD) / 5` |
| 300  | `50ms + 30ms * (5 - OD) / 5`  |

### Approach Rate

*ApproachRate* (AR)决定物件先于标准点多久出现。(标准点即无误差时击打时刻)<!--NC需要改进对"perfect hit"的翻译-->

```
                                        X = 标准点
                p r e e m p t           ↓
 ├───────────────────────┬──────────────┤
 0%      淡入            100% 完全不透明
```

圆圈开始淡入时间为提前标准点`preempt`ms：

- 当 AR < 5: `preempt = 1200ms + 600ms * (5 - AR) / 5`
- 当 AR = 5: `preempt = 1200ms`
- 当 AR > 5: `preempt = 1200ms - 750ms * (AR - 5) / 5`

物件淡入持续多久也取决于AR：

- 当 AR < 5: `fade_in = 800ms + 400ms * (5 - AR) / 5`
- 当 AR = 5: `fade_in = 800ms`
- 当 AR > 5: `fade_in = 800ms - 500ms * (AR - 5) / 5`

### Sliders

```
SliderMultiplier:1.3
SliderTickRate:1
```

*SliderMultiplier* (Decimal)specifies the multiplier of the slider velocity. The velocity at slider multiplier = 1 is 100 osu!pixels per beat. A slider multiplier of 2 would yield a velocity of 200 osu!pixels per beat. The default slider multiplier is 1.4 when the property is omitted.<!--NT-->

*SliderTickRate* (Decimal) is the number of ticks per beat. The default value is 1 tick per beat.<!--NT-->

## Events

### Backgrounds

**语法：** `0,0,filename,xOffset,yOffset`

第一个参数`0`告诉 osu! 这是背景事件。第二个参数决定这个事件的起始时间，不起作用（背景没有起止时间）。

*filename* (String) 记录背景图片的路径<!--NC-->

*xOffset* (Integer) 和 *yOffset* (Integer) 可以调整背景图片至恰当的位置。例如，offset（偏移量）为`50,100`时意味着把背景图片从中央向右移动50 osu!pixel ，向下移动100 osu!pixel。若offset为`0,0`，可以不写 *xOffset* 和 *yOffset* 。

### Videos

**语法：** `Video,time,filename,xOffset,yOffset`

Videos 和 Backgrounds 的语法格式相同，相比之下，第一个参数`0`改为`1`或`Video`告诉osu!这是视频事件。*time* (Integer) 决定视频开始播放的时间。

### Breaks

**语法：** `2,time,endTime`

`2`w或`Break`告诉osu!这是休息事件。

*time* (Integer, 毫秒) 和 *endTime* (Integer, 毫秒) 分别表示一段休息的开始和结束的时刻。

### Storyboards

Storyboards 的配置在另一类扩展名为 *.osb* 的文件里。具体看 [Storyboard 脚本](/wiki/Storyboard_Scripting) 。Storyboard对所有的 *.osu* 谱面都可用。<!--NT原文Storyboards can be defined in a separate optional storyboard file with the *.osb* extension.  See [Storyboard Scripting](/wiki/Storyboard_Scripting). External storyboards are shared between all the *.osu* beatmaps.-->

通过选择是否和外部 Storyboard 链接，可以为特定难度的谱面专门制作 Storyboard。<!--NC-->

## Timing Points

Timing points 记录了有关 BPM 和音效的所有参数。

**语法：** `Offset, Milliseconds per Beat, Meter, Sample Set, Sample Index, Volume, Inherited, Kiai Mode`

*offset* (Integer, 毫秒) 决定歌曲从哪一时刻开始。他决定 Timing Point 从何时开始。新一段 Timing Point 的开始会结束前一段 Timing Point 。第一个 Timing Point在0开始，他没有 offset 。 

Timing Point 由 offset 划分。<!--NT-->

*milliseconds per beat* (Decimal) 决定每节拍多少毫秒。 osu!taiko 和 osu!mania 中的下落速度、 osu!standard 中的滑条速度都受到它的影响。值为正数时，它表达每节拍占毫秒的数值；值为负数时，它表达前一个正数的该参数的百分数。例如，三个连续的 Timing Point 的该参数值分别为`500`，`-50`，`-100`，意味着这三段 Timing Point 各自的节拍占毫秒数为0.5s、0.25s、0.5s。

The *meter* (Integer) 决定一节有几拍。

The *sample set* field defines the default sample set for hit objects. The *sample index* is the default custom index. *Volume* (0 to 100) is the default volume. See the *Hit Objects* section below for details.<!--NT翻译完## Hit Objects后再翻译此行-->

*Inherited* (Boolean: 0 or 1) 是对 *milliseconds per beat* 的补充。当 *milliseconds per beat* 为正、负数时， *Inherited* 各取1，0。

*kiai mode* (Boolean) 决定这段 Timing Point 是否为 [Kiai Time](/wiki/Beatmap_Editor/Kiai_Time) 状态。

 Timing Point的一个例子：

`66,315.789473684211,4,2,0,45,1,0`

继承型 Timing Point 的一个例子:

`10171,-100,4,2,0,60,0,1`

## Colours

### Combos

combo 的颜色决定`Combo1`至`ComboN`的颜色。

每一个颜色格式为RGB，取值范围为0\~255。

以两个 combo 为例，第一个为淡灰色，第二个为红色。

```
Combo1 : 245,245,245
Combo2 : 255,0,0
```

每组 combo 永远从1开始、分界明确且连续不断，其他情况都无效。<!--NC需要确认"其他情况都无效。"的翻译，原文"Any other order is an undefined behavior."-->

一轮 combo 的颜色轮完后，新一轮的 combo 颜色仍沿用这套顺序。在本例中，第三组 combo 为灰色，第四组为红色。

### Special colours

下述参数是滑条特有的可选自定义参数：

- `SliderBody`,
- `SliderTrackOverride`,
- `SliderBorder`.

和 combo 的颜色一样，这些参数都是RGB格式。

combo 的颜色不会作用于特有颜色。

## Hit Objects

### Common structure

这一部分使用 CSV 编写。前五个是所有物件的基础属性，最后一个 *extras* 为可选参数。

**语法**： `x,y,time,type,hitSound...,extras`

#### Position

*x*、 *y*(Integer) 决定物件中心的坐标。 *x* *y* 的范围各为0\~512 osu!pixel 和 0\~384 osu!pixel 。原点(0,0)在屏幕的左上角。

为了统一为在标准分辨率 640x480 中确定物件的坐标，你需要将 *x* 加上 64 像素，将 *y* 加上 48 像素。 如果没有选定坐标，物件将留在(0,0)左上角。

对于部分物件，比如转盘，坐标没有意义。

对于 osu!mania ，只有 *x* 有意义。具体内容在 osu!mania hold note 中。

#### Time

*time*(Integer、毫秒) 决定物件在时间上的位置。

#### Type

*type* is a bitmap specifying the object type and attributes.<!--NT-->

- Bit 0 (1): 圆圈。
- Bit 1 (2): 滑条。
- Bit 2 (4): 新一组 combo。
- Bit 3 (8): 转盘。
- Bits 4-6 (16, 32, 64) form a 3-bit number (0-7) that chooses how many combo colours to skip.<!--NT-->
- Bit 7 (128) 是 osu!mania 中的长按。

圆圈，滑条，转盘和长按都可以和新开 combo (即Bit 2)、跳过 combo 颜色(即Bit 4-6)共存，但互相不能共存。<!--NT原句Circles, sliders, spinners, and hold notes can be OR'd with new combos and the combo skip value, but not with each other.-->

The new combo flag always advances to the next combo. The skip value is applied on top of that, so that a skip of 1 means a 2-combo advance. The combo skip value is ignored when the new combo bit is not set.

例如：

- `1`: 一个圆圈。
- `5 = 1 + 4`: 新开一组 combo 的圆圈。
- `22 = 2 + 4 + 16`: 新开一组 combo 的滑条，跳过了两组颜色。

#### Hit sounds

*hitSound* (Integer) is a bitmap of hit sounds to play when the hit object is successfully hit.

- Bit 0 (1): normal.
- Bit 1 (2): whistle.
- Bit 2 (4): finish.
- Bit 3 (8): clap.

The normal sound is always played, so bit 0 is irrelevant today. The only exception is for osu!mania, with the skin's *LayeredHitSounds* property.

Multiple sounds will overlap if multiple bits are set.

The sample set and custom index are usually specified in the timing point associated to the hit object, but may be customized in the *extras* field.

The normal hit sound and additions may belong to different sample sets, referred to as *sampleSet* and *additionSet*.

The filename of the sample to play is `{sample set}-hit{sound}{index}.wav`, where:

- *sample set* is normal, soft, or drum.
- *sound* is normal, whistle, finish, or clap.
- *index* is the custom index. It is omitted when equal to 0 or 1.

The loader searches for the sample file in one these directories, by order of priority:

1. Inside the beatmap directory with its index, *unless* the custom index 0.
2. Inside the skin directory, without the index.
3. Inside the default osu! resources, without the index.

#### Extras

*extras* 作为可选参数，决定additional parameters related to the hit sound samples. 默认值为 `0:0:0:0:`。

**语法**： `sampleSet:additionSet:customIndex:sampleVolume:filename`

*sampleSet* (Integer) changes the sample set of the normal hit sound, and *additionSet* (Integer) changes the sample set for the other hit sounds (whistle, finish, clap). The values for these are:

- 0: Auto. See below.
- 1: Normal.
- 2: Soft.
- 3: Drum.

When *sampleSet* is 0, its value is inherited from the timing point.

Today, *additionSet* inherits from *sampleSet*. Otherwise, it inherits from the timing point.

*customIndex* (Integer) is the custom sample set index, e.g. 3 in `soft-hitnormal3.wav`. The special index 1 doesn't appear in the filename, for example `normal-hitfinish.wav`. The special index 0 means it is inherited from the timing point.

*sampleVolume* (Integer) is the volume of the sample, and ranges from 0 to 100 (percent).

*filename* (String) names an audio file in the folder to play instead of sounds from sample sets, relative to the beatmap's directory.

### Hit Circles

Hit Circles 即单个物件。

**语法**： `x,y,time,type,hitSound,extras`

**例子**： `164,260,2434,1,0,0:0:0:0:`

### Sliders

Slider 在 Catch the Beat 中为一串水果； osu!taiko 中为黄色物件<!--NC-->； osu!mania 中没有 Sliders 。

**语法**： `x,y,time,type,hitSound,sliderType|curvePoints,repeat,pixelLength,edgeHitsounds,edgeAdditions,extras`

**例子**： `424,96,66,2,0,B|380:120|332:96|332:96|304:124,1,130,2|0,0:0|0:0,0:0:0:0:`

#### Path

*sliderType* will be `L` (linear), `P` (perfect), `B` (Bezier), or `C` (Catmull, deprecated).

*curvePoints (x:y|...)* is a series of `|`-separated coordinates describing the control points of the slider.

A **linear** slider has a start, specified in *x* and *y* from the common fields, and an end point specified in *curvePoints*. For example `L|100:200`.

A **perfect** circle slider is defined by three points. In that order: start, pass-through, and end. *x* and *y* define the start point, and *curvePoints* defines the pass-through and end point. For example `P|250:200|200:15`.

A perfect circle slider could be represented as a center point, a radius, and two angles for convenience. See this source code for the conversion algorithm: [PathApproximator.cs](https://github.com/ppy/osu-framework/blob/master/osu.Framework/MathUtils/PathApproximator.cs).

A **Bézier** slider is made of one or many Bézier curves, sharing common ends. The degree of each curve is arbitrary. The first control points is defined with *x* and *y*, and the other ones by *curvePoints*.

To identify the separation between two curves, the intersection point is repeated. Consider the sequence ABCDDEFFG. You would get the 3 Bézier curves: ABCD (cubic), DEF (quadratic) , FG (linear).

Example: `476,340,6419,2,0,B|437:336|422:309|422:309|384:309|359:337|359:337|328:308|300:304|300:304|272:352|237:383|176:356|159:287|224:256,1,420,6|2,0:0|0:0,0:0:0:0:`

The first Bézier curve in the segment is quadratic with the following points: (476, 340), (437, 336), (422, 309).

#### Repeat

*repeat* (Integer) is the number of times a player will go over the slider. A value of 1 will not repeat, 2 will repeat once, 3 twice, and so on.

#### Length and duration

*pixelLength* (Decimal) is the length of the slider along the path of the described curve. It is specified in osu!pixels, i.e. relative to the 512×384 virtual screen.

The *pixelLength* is not the length of the curve path described above, but the actual length the slider should have. If the *pixelLength* is smaller than the path length, the path must be shrinked. Conversely, if the *pixelLength* is bigger than the path length, the path must be naturally extended: a longer line for linear sliders, a longer arc for perfect circle curves, and a final linear segment for Bézier paths.

The *pixelLength* is notably used to compute the duration of the slider. To get the slider duration, use the following formula:

`slider duration = pixelLength / (100.0 * SliderMultiplier) * BeatDuration`

Where:

- *SliderMultiplier* is the property defined in the `[Difficulty]` section.
- *BeatDuration* is the duration of a beat, specific to the current timing point.

The duration you will get is in the same unit as *BeatDuration*, usually milliseconds.

#### Sounds

*hitSound* applies only to the body of the slider. Only *normal* (0) and *whistle* (2) are supported. The samples played are named like `soft-sliderslide4.wav` for normal, and `normal-sliderwhistle.wav` for whistle. These samples are meant to be looped, and may also be empty WAV files to mute the slider.

*edgeHitsounds (hitSound|...)* is a `|`-separated list of *hitSounds* to apply to the circles of the slider. The values are the same as those for regular hit objects. The list must contain exactly *repeat + 1* values, where the first value is the hit sound to play when the slider is first clicked, and the last one when the slider is released.

*edgeAdditions (sampleSet:additionSet|...)* is a `|`-separated list of samples sets to apply to the circles of the slider. The list contains exactly *repeat + 1* elements. *sampleSet* and *additionSet* are the same as for hit circles' *extras* fields.

When *sampleSet* is 0, it inherits from the *sampleSet* in the *extras* field of the hit object, and then from the timing point. *additionSet* inherits from the *additionSet* in *extras*, then the timing point.

The final *extras* defines the sample to use on the slider body. It functions like *extras* for a circle.

### Spinners

**Syntax**: `x,y,time,type,hitSound,endTime,extras`

**Example**: `256,192,730,12,8,3983`

Spinner 在 Catch the Beat 中为香蕉雨；osu!taiko 中的转盘。osu!mania 中没有 Spinner。

*endTime (Integer)* is when the spinner will end, in milliseconds from the beginning of the song.

Hit sounds play at the end of the spinner.

### osu!mania Hold Notes

A hold note unique to osu!mania.

**Syntax**: `x,y,time,type,hitSound,endTime:extras`

**Example**: `329,192,16504,128,0,16620:0:0:0:0:`

*x* (Integer) 决定长条在第几列落下。 *y* 无意义。

The number of column is defined by the *CircleSize* property in the Difficulty section. Columns are indexed from 0.<!--NT-->

The column for a note is computed with `x / column width` with `column width = 512 / number of columns`. The resulting value is floored, then clamped between 0 and (#column - 1) for safety.

To avoid rounding errors, *x* is best picked in the middle of the range for its column. For example, in 4K mode, the first column ranges from 0 to 128, so the safest value for x is 64.

For the 7K + 1 mode, the column index is `1 + x / (512 / 7)`, leaving the column 0 for the specials.

*endTime* (Integer、毫秒) 长按的终止时刻，数值为歌曲开始到终止的毫秒数。

<!--NC:### Common structure需要更好的翻译，涉及CSV内容-->
