# Compressing Files

Osu! maps, according to the current ranking guidelines, must be under 10 MB, or 24 MB if the song has a video. In this tutorial I will tell you smart ways to get your map under that limit.

There are 2 types of compression. **Lossy** and **Lossless** compression.

-   **Lossless** implies that the quality never degrades and can be repeatedly compressed or decompressed.
-   **Lossy** is a much more powerful form of compression which sacrifices quality for space/processor demand.

Zip
---

The `.osz` package is actually a `.zip` file, and will compress your beatmap, although not very much, since audio, video, and images are usually compressed very well. Zip and other archives are all lossless compression, otherwise you wouldn't be able to get your data back.

Video
-----

Recommended reading: [Encoding Video](/wiki/Beatmap_Editor_Guides/Compressing_Videos).

Videos are usually where people go wrong. There are thousands of video codecs out there, and *believe it or not, YouTube is usually a terrible place to get videos*. For the best quality, you should always downsize from a high resolution source (720p YouTube videos are fine for this).

h.264 and XviD are very good codecs to use but like most video codecs, they are lossy. So do not re-encode multiple times, but encode from the high resolution source.

Audio
-----

Now that there is a limit on audio bitrate, it's not as much of a problem anymore. However long songs at 192 kbps will undoubtedly take up most of your space. I recommend using a variable bitrate between rate factor 2 and 5 (I try to stick around 4). With a variable bitrate, you get more compression in low activity areas, and more quality in higher areas.

![Compressing Audio](CBF_01.png "Compressing Audio")

Programs such as [Audacity 1.3.13](http://audacity.sourceforge.net/download/) does an excellent job of saving variable bitrate audio with the correct plugins.

Osu accepts 2 major file formats: mp3 and ogg vorbis. Vorbis has a clear advantage over mp3 at low bitrates (under 128 kbps), but suffers from lack of support by proprietary software like apple, since mp3 is the standard for audio. However, there are severely limiting returns on using anything higher than 128 kbps. For osu! it doesn't really matter which one you use.

Images
------

There are 2 major image formats which make up most of the images you find online: jpg and png. Png uses lossless compression which makes it ideal for small and or simple images. Complex images are better suited for jpg. The majority of image editing programs however do not naturally use `.png` and `.jpg` compression to the most of their ability however, leaving you with 4 KB pngs of 1 color, which could be compressed up to 400 times smaller.

[GIMP](http://www.gimp.org/) actually does a good job with `.jpg` files.

![Compressing Images](CBF_02.png "Compressing Images")

There are four important things to check: Optimize, Progressive, subsampling, and quality. Optimize is just a way to compress the `.jpg` without losing quality and should always be checked. Progressive is a method to make jpgs "fade in" when downloaded from the internet. It has a side effect of making the image smaller so long as the image is over 20 KB. Subsampling is a way to improve quality or compression. No subsampling (1x1) will make text and lines much clearer at the cost of space. 2x2 subsampling does very well for photographs which do not have distinct lines (like text). Quality is the easiest way to keep the image looking good. I use 95, since the gains after 95 aren't really worthwhile.

PNGs are actually much simpler to compress, but GIMP does not do it very well. [OptiPNG](http://optipng.sourceforge.net/) and [PNGOUT](http://advsys.net/ken/utils.htm) are two of the best tools to compress `.png` files. OptiPNG can find the optimum settings for the `.png`, and PNGOUT re-compresses the image using `.kzip`. Often times just using PNGOUT will reduce the image size by 20%.

![Compressing Images with PNGOUT](CBF_03.png "Compressing Images with PNGOUT")

For even better compression, you can use a script which combines multiple compressors and brute forces close to the smallest file possible. The script's name is [pngslim](http://people.bath.ac.uk/ea2aced/tech/png/pngslim.zip).

![Compressing Images with pngslim](CBF_04.png "Compressing Images with pngslim")

Results
-------

Here we have results of compressing.

![Compression Results](CBF_05.png "Compression Results")

Compressing Videos
=====================

Precursor/Notes
---------------

Editing videos with [avidemux](http://fixounet.free.fr/avidemux/download.html)

Removing audio
--------------

1) Open avidemux

2) Drag and drop the file into avidemux

3) If the following shows up because the video is h.264 (h.264 is the best right now):

   a) Press either (no is better unless the program crashes).

![Tutorial Image 1](CV_01.png "Tutorial Image 1")

4) Select Audio -> Main Track

![Tutorial Image 2](CV_02.png "Tutorial Image 2")

5) Select Audio Source -> None

![Tutorial Image 3](CV_03.png "Tutorial Image 3")

Encoding Video
--------------

6) Make sure that both the video and audio are on "Copy".

![Tutorial Image 4](CV_04.png "Tutorial Image 4")

7) If you want to instead re-encode the file, then choose "MPEG-4 AVC" to pick h.264. Note that…

*mm201 wrote:* h.264 lags single-core machines like crazy and shouldn't be used. I do not agree with this, as we have a video toggle, and this isn't 2005. If you want to support ancient PCs, then use h.263 or Xvid.

![Tutorial Image 5](CV_05.png "Tutorial Image 5")

8) To resize the image, click on "filters" and "MPlayer resize" then input how much you want to resize. Most of the time you should keep this at 800x600 or 853x480 (though I use 800x450 for widescreen).

![Tutorial Image 6](CV_06.png "Tutorial Image 6")

9) To actually reduce the filesize of the video, there are a few options, all of which are in the "configure" menu

![Tutorial Image 7](CV_07.png "Tutorial Image 7")

10) The correct way is to use a constant rate factor (usually between 30-36) since single pass encodes are of higher quality. You can also use a 2 pass encode which will set the video size (I suggest ~7 MB) or Average bitrate (I suggest 400-800 kbps). Avidemux doesn't like saving h.264 flv files, but works fine with avi files. Since osu plays both just fine (and avi is slightly smaller than flv), save the file as an avi.

![Tutorial Image 8](CV_08.png "Tutorial Image 8")

Save
----

11) Press `Ctrl` + `S` to save the file somewhere, then copy it into your folder.

Final Remarks
-------------

If avidemux does not open your file correctly, there are alternatives: [Mediacoder](http://www.mediacoderhq.com/) is a bit more difficult to use, but might work, and can save h.264 flv files. [SUPER](http://www.erightsoft.com/SUPER.html) isn't very good, hard to find, but is another program that might be worthwhile, if you can find the download on the website. Finally, [VLC](http://www.videolan.org/vlc/) can be used, **but that should be avoided at all costs**.

The reason I like avidemux is because you can easily edit each frame, and it has a good interface, unlike mediacoder (which has greater compatibility). I've never been able to get virtualdub to work properly.


## Trivia

- Original forum posts:
  - [*How to make your map fit the size limitations: Compression* by: ziin](https://osu.ppy.sh/forum/t/60002)
  - [*How to re-encode/edit a video* by: ziin](https://osu.ppy.sh/forum/t/58235)
