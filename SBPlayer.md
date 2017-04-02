## macOS 增加一款支持全格式、界面时尚、播放流畅的视频播放器

> 历时2个月的时间，终于设计和开发完成一款符合自己要求的视频播放器。在开发这款播放器之前，我对播放器的期望是：这款播放器的界面一定不能和Mac AppStore上绝大多数视频播放器那样界面丑陋，极度不够人性化，而且要符合国人的口味，界面皮肤可以更换，让喜欢不同颜色界面的人都能找到自己喜欢的样式，速度要快，支持几乎所有格式。正所谓好马配好鞍，为了适配优雅细腻的macOS，所以就开发了SBPlayer。

##### SBPlayer适配多国语言，支持繁简中文、英语、法语、西班牙语、日语。

#### SBPlayer的优点：
1.几乎支持所有本地视频和音频格式，国人看片经常用到的格式更是完美支持。
2.切换播放以及打开文件速度极快，几乎毫不卡顿，支持拖拽文件到窗口播放，打开文件按钮播放，快捷键打开文件播放，支持键盘控制进度，声音，播放/暂停，下一个视频等等，支持按住播放器随意移动，自动关联相关文件格式，播放4k等视频毫无压力。
3.界面美观，一改Mac端播放器普遍界面单一，绝大多数无法更换皮肤，对喜欢不同颜色的用户来说是个遗憾，SBPlayer提供多种皮肤供用户选择。
4.SBPlayer主打本地视频播放，剔除普通用户用不到的一些功能，精简播放器，使用更为简单明了。

##### SBPlayer部分功能截图：

![QQ20170317-155715.png](http://upload-images.jianshu.io/upload_images/2105518-6efb3d54660e57c8.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![QQ20170317-155726.png](http://upload-images.jianshu.io/upload_images/2105518-43149571d778474e.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![QQ20170317-155648.png](http://upload-images.jianshu.io/upload_images/2105518-812640b51abb7691.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![QQ20170317-155746.png](http://upload-images.jianshu.io/upload_images/2105518-9ee316851ca6daa0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


![QQ20170321-155720.png](http://upload-images.jianshu.io/upload_images/2105518-24bee471e3bf0dae.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

#### SBPlayer支持几乎所有本地视频格式，包含但并不止如下格式：

*webm.*rmvb.*.asf *.avi *.divx *.dv *.flv *.gxf *.m1v *.m2v *.m2ts *.m4v *.mkv *.mov *.mp2 *.mp4 *.mpeg *.mpeg1 *.mpeg2 *.mpeg4 *.mpg *.mts *.mxf *.ogg *.ogm *.ps *.ts *.vob *.wmv *.a52 *.aac *.ac3 *.dts *.flac *.m4a *.m4p *.mka *.mod *.mp1 *.mp2 *.mp3 *.ogg等等由于是基于VLC所开发的播放器，所以理论上VLC支持的格式SBPlayer也完全支持，SBPlayer也可以播放视频流格式，HTTP、RTMP、m3u8、mms等等格式，不过rtsp格式暂时还有点问题。

#### 浅谈对滥用第三方库的看法

作为本地视频播放格式个人感觉非常完美,SBPlayer除去用的第三方库，总共代码1000多行，不到2000行，但依然超出了自己的预计的代码量，用OC还是挺耗行数的，另外自己逻辑能力还不够强，多增加了不少代码。OC用久了，形成了依赖，但更喜欢Swift,期待更稳定的Swift4.0发布，让代码变的少之又少。一个程序员代码写的太多绝不是优秀的程序员，更有点逻辑混乱的意味。未来开发对自己的要求是尽量少用或者不用第三方库，很多功能很简单完全没必要用太复杂的库，比如网络请求AFNetworking,一般网络请求自己写一个代码更少，网络缓存之类的都很好做，出了Bug可以很好的定位。还有关于约束，比较有名的就Masonry和SDAutolayout,然而毕竟是第三方库，自从ios9后苹果新增加了一种类似于Masonry的约束框架，完全可以媲美Masonry，当ios11快出来后，最低开发版本就可以定位ios9，Masonry也就没什么必要了，另外等Swift再次更新时，相信SBAutolayout再简便，Swift系统自带约束也完全可以替代。在很早之前UITableView和UICollectionView的动态cell行高，用系统方法一行或者二行代码就可以搞定，很好奇为什么UITableView-FDTemplateLayoutCell这个自动约束的第三方库为什么这么多人用，系统能一步解决的问题，为什么还要下载个庞大的第三方库复杂的完成它。很多有名第三方库，在那些作者开发时也许很有必要，但iOS sdk本身就是个动态改进和升级的过程，以前难解决的问题，系统已经加入更好的方法完成它，这些第三方库或许已经完成了它的历史任务，再用它就显得画蛇添足了。


>对喜欢换个口味的用户到时候可以试试看。

最近做的一个用Swift写的开源的mac端cocoapods助手很快也将做完，使用它让利用cocoapods导入第三方库将更简单



[返回](./)
