## 2.1 P2P会议模块 Android 端SDK概述



Android版的P2P会议模块是在Android版的Peergine中间件\(JNI插件\)的基础上封装出来的一个java类。Peergine中间件的功能强大，API接口复杂，需要经过较长时间的学习才能掌握。现在在Peergine中间件的基础上封装出一个P2P会议类，API接口大大简化，方便于开发者的使用。P2P会议类的源代码在pgLibConference\App\Android目录中。Android版的Peergine中间件以两种方式提供：单独的APK和库工程。

1）单独的APK：Peergine中间件是一个单独的APK，单独安装，不需要合并到APP的APK。安装APP的APK的Android设备上，必须也要安装Peergine中间件的APK，才能正常使用。Peergine中间件的APK在pgLibConference\Plugin\APK目录中。

2）库工程：Peergine中间件的库工程。把此库工程导入到eclipse的workspace中（与APP的工程同一个workspace），然后在APP的工程中引用此库工程（如何引用库工程请在网络上找教材）。编译APP的工程时就会把库工程打包在一起，合成一个APK。库工程在pgLibConference\Plugin\AndroidLib目录中。



