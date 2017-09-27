## macOS 增加一款支持全格式、界面时尚、播放流畅的视频播放器

> 历时2个月的时间，终于设计和开发完成一款符合自己要求的视频播放器。在开发这款播放器之前，我对播放器的期望是：这款播放器的界面一定不能和Mac AppStore上绝大多数视频播放器那样界面丑陋，极度不够人性化，而且要符合国人的口味，界面皮肤可以更换，让喜欢不同颜色界面的人都能找到自己喜欢的样式，速度要快，支持几乎所有格式。正所谓好马配好鞍，为了适配优雅细腻的macOS，所以就开发了SBPlayer。

##### SBPlayer适配多国语言，支持繁简中文、英语、法语、西班牙语、日语。

#### SBPlayer的优点：
1. 几乎支持所有本地视频和音频格式，国人看片经常用到的格式更是完美支持。
2. 切换播放以及打开文件速度极快，几乎毫不卡顿，支持拖拽文件到窗口播放，打开文件按钮播放，快捷键打开文件播放，支持键盘控制进度，声音，播放/暂停，下一个视频等等，支持按住播放器随意移动，自动关联相关文件格式，播放4k等视频毫无压力。
3. 界面美观，一改Mac端播放器普遍界面单一，绝大多数无法更换皮肤，对喜欢不同颜色的用户来说是个遗憾，SBPlayer提供多种皮肤供用户选择。
4. SBPlayer主打本地视频播放，剔除普通用户用不到的一些功能，精简播放器，使用更为简单明了。

##### SBPlayer部分功能截图：

![QQ20170317-155715.png](http://upload-images.jianshu.io/upload_images/2105518-6efb3d54660e57c8.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![QQ20170317-155726.png](http://upload-images.jianshu.io/upload_images/2105518-43149571d778474e.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![QQ20170317-155648.png](http://upload-images.jianshu.io/upload_images/2105518-812640b51abb7691.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![QQ20170317-155746.png](http://upload-images.jianshu.io/upload_images/2105518-9ee316851ca6daa0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


![QQ20170321-155720.png](http://upload-images.jianshu.io/upload_images/2105518-24bee471e3bf0dae.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

#### SBPlayer支持几乎所有本地视频格式，包含但并不止如下格式：

*webm.*rmvb.*.asf *.avi *.divx *.dv *.flv *.gxf *.m1v *.m2v *.m2ts *.m4v *.mkv *.mov *.mp2 *.mp4 *.mpeg *.mpeg1 *.mpeg2 *.mpeg4 *.mpg *.mts *.mxf *.ogg *.ogm *.ps *.ts *.vob *.wmv *.a52 *.aac *.ac3 *.dts *.flac *.m4a *.m4p *.mka *.mod *.mp1 *.mp2 *.mp3 *.ogg等等由于是基于VLC所开发的播放器，所以理论上VLC支持的格式SBPlayer也完全支持，SBPlayer也可以播放视频流格式，HTTP、RTMP、m3u8、mms等等格式，不过rtsp格式暂时还有点问题。


>对喜欢换个口味的用户到时候可以试试看。
>> 源码： [https://github.com/shibiao/SBPlayerClient](https://github.com/shibiao/SBPlayerClient)

>> 下载地址:[SBPlayer_V1.2](https://pan.baidu.com/s/1mhRmVfM) (>=10.12)

最近做的一个用Swift写的开源的mac端cocoapods助手很快也将做完，使用它让利用cocoapods导入第三方库将更简单



[返回](./)
