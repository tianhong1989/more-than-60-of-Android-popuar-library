# more-than-60-of-Android-popuar-library
2018年60个实用Android框架排行榜


1.Retrofit
一句话介绍：Retrofit是一款类型安全的网络框架，基于HTTP协议，服务于Android和java语言

上榜理由：Retrofit以21.8k的stars量雄踞github中android子标题榜首，第一当之无愧。

官网地址 http://square.github.io/retrofit/

github   https://github.com/square/retrofit

作者：square团队

使用：

compile 'com.squareup.retrofit2:retrofit:2.3.0'
2.okhttp

一句话介绍：okhttp是一款基于HTTP和HTTP2.0协议的网络框架，服务于java和android客户端

上榜理由，okhttp以20.4k的stars量雄踞github中android子标题第二名。大型公司比如淘宝也封装的是okhttp。Retrofit2.0开始内置okhttp框架，Retrofit专注封装接口完成业务需求，okhttp专注网络请求的安全高效，笔者将两者区分开，是想让后来学习者知道，这是两套框架，学习框架原理时可以分开学习，以免理解混乱。

官网地址   http://square.github.io/okhttp/

github    https://github.com/square/okhttp

作者：square团队

使用：

compile 'com.squareup.okhttp3:okhttp:3.9.1'
3.Butter Knife


一句话介绍：Butter Knife所提供了一种能力——使用注解生成模板代码，将view与方法和参数绑定。

上榜理由：github上16.5K个star，配合Androidstudio提供的Butter Knife插件，帮助开发者省却了频繁findviewbyid的烦恼，最新的Butter Knife还提供了onclick绑定以及字符串的初始化，初学者可以查阅Butter Knife以及Butter Knife插件进一步学习！

官网地址：http://jakewharton.github.io/butterknife/

github：https://github.com/JakeWharton/butterknife

作者：JakeWharton ，也是square团队成员之一

使用：

dependencies {  compile 'com.jakewharton:butterknife:8.8.1'  annotationProcessor     'com.jakewharton:butterknife-compiler:8.8.1'}
4.MPAndroidChart


一句话介绍：MPAndroidChart是一款图表框架

上榜理由：github上16.1K个star，以快速、简洁。强大著称的图表框架

官网地址 https://github.com/PhilJay/MPAndroidChart  

github  https://github.com/PhilJay/MPAndroidChart

作者：PhilJay

使用：

在AS中加入Gradle依赖

在根目录的 build.gradle上加入:

allprojects {    repositories {        maven { url "https://jitpack.io" }    }}
在app的build.gradle上加入：

dependencies {    compile 'com.github.PhilJay:MPAndroidChart:v3.0.3'}
5.glide


一句话介绍：glide是一款专注于提供流畅划动能力的“图片加载和缓存框架”

上榜理由：15.9k个star，图片加载类框架排名第一的框架，google 在2014开发者大会上演示的camera app就是基于gilde框架开发的

github https://github.com/bumptech/glide

作者 Bump Technologies团队

使用：

repositories {  mavenCentral()}dependencies {    implementation 'com.github.bumptech.glide:glide:4.5.0'    annotationProcessor 'com.github.bumptech.glide:compiler:4.5.0'}
6.leakcanary


一句话介绍：一款内存检测框架，服务于java和android客户端

上榜理由：方便，简洁是leakcanary最大的特点，只需在应用的apllication中集成，就可以直接使用它；15.5k个star说明了它有多么受欢迎

github https://github.com/square/leakcanary

作者 square团队

使用：

 dependencies {   debugCompile 'com.squareup.leakcanary:leakcanary-android:1.5.4'   releaseCompile 'com.squareup.leakcanary:leakcanary-android-no-op:1.5.4'   testCompile 'com.squareup.leakcanary:leakcanary-android-no-op:1.5.4' }
在 Application 中写入:

public class ExampleApplication extends Application {  @Override public void onCreate() {    super.onCreate();    if (LeakCanary.isInAnalyzerProcess(this)) {      // This process is dedicated to LeakCanary for heap analysis.      // You should not init your app in this process.      return;    }    LeakCanary.install(this);    // Normal app init code...  }}
7.Android-Universal-Image-Loader


一句话介绍：曾经的图片加载框架王者，android开发老手都用过它

上榜理由:android端图片加载框架的老大哥了，15.3k个star足以证明它的热门，UIL与gilde最大区别是可定制，UIL提供了大量配置方式，图片加载状态的回调（成功，失败，进行中），加载动画等；以及提供了移动端图片加载框架的缓存思路：三级缓存策略 sd卡-内存-网络；值得注意的是，UIL以及两年未更新了，但笔者仍推荐各位使用！

github https://github.com/nostra13/Android-Universal-Image-Loader

作者 nostra13

使用：

下载地址  universal-image-loader-1.9.5.jar

8.EventBus


一句话介绍：EventBus是一款本地组件间通信框架

上榜理由：组件间通信框架star量第一：14.8k，在大型项目的Activities，fragments，Threads，Services都可以看到它的使用场景，尽管EventBus在向未创建的组件传递事件时有些局限，仅适合在“活着的”组件间传递消息，但仍不妨碍它活跃在各个大型项目各个场景里。

官网地址 http://greenrobot.org/eventbus/documentation/how-to-get-started/

github  https://github.com/greenrobot/EventBus

作者 greenrobot

使用：

compile 'org.greenrobot:eventbus:3.1.1'
9.zxing


一句话介绍：条码图像处理库

上榜理由：如果你用过二维码，你肯定已经间接使用过大名鼎鼎的zxing了。13.9K的star量，让它排在本榜单第九，实至名归，如果你有了解二维码的需求，不妨从了解、修改它源码入手。

github  https://github.com/zxing/zxing

作者  Sean Owen

10.picasso


一句话介绍：强力的图片下载、缓存框架

上榜理由：本榜单出现的第三款图片类框架，不同的是picasso更强调图片下载，你可以将picasso集成进你的项目中，你也可以结合gilde和UIL与picasso，三者一齐封装至你的项目中，按需所用。

官网地址 http://square.github.io/picasso/

github  https://github.com/square/picasso

作者 square团队

使用：

compile 'com.squareup.picasso:picasso:2.5.2'
或者下载jar包

11.lottie-android


一句话介绍：一款可以在Android端快速展示Adobe Afeter Effect（AE）工具所作动画的框架

上榜理由：动画类框架第一名，github上13.3k个star证明了他的优越性，利用json文件快速实现动画效果是它最大的便利，而这个json文件也是由Adobe提供的After Effects（AE）工具制作的，在AE中装一个Bodymovin的插件，使用这个插件最终将动画效果生成json文件，这个json文件即可由LottieAnimationView解析并生成绚丽的动画效果。而且它还支持跨平台哟。

github  https://github.com/airbnb/lottie-android

作者：Airbnb 团队

12.fresco


一句话介绍：一款可以管理图片内存的框架

上榜理由:github上12.8k个star，图片类排行榜第四名，facebook的出身证明了它并非是重复造的轮子，在管理图片内存领域上有着它的一片天地，渐进式加载、加载gif都是它与前三位相比独有的特性

官网地址： https://www.fresco-cn.org/

github  https://github.com/facebook/fresco

作者 facebook

使用：

dependencies {  // 其他依赖  compile 'com.facebook.fresco:fresco:0.12.0'}
下面的依赖需要根据需求添加：

dependencies {  // 在 API < 14 上的机器支持 WebP 时，需要添加  compile 'com.facebook.fresco:animated-base-support:0.12.0'  // 支持 GIF 动图，需要添加  compile 'com.facebook.fresco:animated-gif:0.12.0'  // 支持 WebP （静态图+动图），需要添加  compile 'com.facebook.fresco:animated-webp:0.12.0'  compile 'com.facebook.fresco:webpsupport:0.12.0'  // 仅支持 WebP 静态图，需要添加  compile 'com.facebook.fresco:webpsupport:0.12.0'}
13.RxAndroid


一句话介绍：一款Android客户端组件间异步通信的框架

上榜理由：github上12.7k个star，位居组件通信框架的第二名，仅在EventBus之后，如果要问两者的区别，Eventbus是用来取代组件间繁琐的interface，RxAndroid是用来取代AnsyTask的，并不冲突；当然RxAndroid的优点并不仅限于此，更多优雅的实现，可以去官网查阅！

github  https://github.com/ReactiveX/RxAndroid

作者 JakeWharton

使用：

compile 'io.reactivex.rxjava2:rxandroid:2.0.1'compile 'io.reactivex.rxjava2:rxjava:2.1.0'
14.SlidingMenu

一句话介绍：侧滑菜单栏框架

上榜理由：与Userval-Image-loader 齐名的上古神器框架——为你的app提供侧滑菜单栏的功能；github闪更有10.5k个star，证明了它的经久不衰，即使在Google推出了NavigationDrawer，仍然没有减少开发者对SildingMenu的拥簇，经典总是经得起考验的，这个上古神兽已经四年没有更新了；有太多太多的app使用过它，这些都可以在软件的开源许可上看到！

github https://github.com/jfeinstein10/SlidingMenu

作者 Jeremy Feinstein

使用：

在gihub上fork源码，集成进项目中

15.PhotoView

一句话介绍：一款ImageView展示框架，支持缩放，响应手势

上榜理由：10.3k的star数量，位于图片类框架排行榜第五位，PhotoView与前四位不同的是这次带来的是图片的展示能力，你一定好奇微信的头像点击放大是如何实现的，很多App的图片显示响应手势按压是如何实现的，了解PhotoView，你一定会开心的！（笔者也不会告诉你ImageView的点击放大效果在Android的sample也有）

github  https://github.com/chrisbanes/PhotoView

作者：chrisbanes

使用：

在app根目录的build.gradle中加入：

allprojects {    repositories {        maven { url "https://jitpack.io" }    }}
在app的module目录的build.gralde中加入：

dependencies {    compile 'com.github.chrisbanes:PhotoView:latest.release.here'}
使用

<com.github.chrisbanes.photoview.PhotoView    android:id="@+id/photo_view"    android:layout_width="match_parent"    android:layout_height="match_parent"/>PhotoView photoView = (PhotoView) findViewById(R.id.photo_view);photoView.setImageResource(R.drawable.image);
16.material-dialogs

一句话介绍：一款自定义dialog框架

上榜理由：9.9k个star，也是继PhotoView，SlidingMenu之后第三款自定义View框架，也许你还是自定义View的新人，对Dialog使用的还有点生疏，你可以通过它提升你的Dilaog使用能力

github  https://github.com/afollestad/material-dialogs

作者：Aidan Follestad

使用：

dependencies {    // ... other dependencies here    compile 'com.afollestad.material-dialogs:core:0.9.4.5'}
17.droid-async-http

一句话介绍：一款基于Http协议的异步请求的网络框架，

上榜理由：虽然你有无数个使用retrofit+okhttp的理由，但9.8k个star，证明它仍然值得你深入学习。值得注意的是，它也已经有两年没更新了，你尽管拿去当你懒惰的理由！

github   https://github.com/loopj/android-async-http

作者：James Smith

使用：

repositories {  maven {    url 'https://oss.sonatype.org/content/repositories/snapshots/'  }}dependencies {  compile 'com.loopj.android:android-async-http:1.5.0-SNAPSHOT'}
18.androidannotations

一句话介绍：一款基于注解的快速开发框架

上榜理由：与Butterknife一样基于注解，利用注解快速完成view的初始化，不同的是androidannotations提供了更多的能力：简单的线程模型等；笔者只接触过Butterknife，无法更进一步叙述androidannotations的优势，如果你志在深入了解注解的妙用，可以尝试探索一下！

官网地址 http://androidannotations.org/

github https://github.com/androidannotations/androidannotations

作者： WonderCsabo



19.fastjson

一句话介绍:一款基于json解析、生成的框架

上榜理由：从它的名字不难看出，快速是它最大的特性，阿里巴巴的出身保证了代码的质量和优越，9.4k的star数量，也是榜单里第一个出现的中国开源框架，涉及网络的app都会用到json，fastjson值得作为你的首选！

github  https://github.com/alibaba/fastjson

作者：alibaba

使用：

compile 'com.alibaba:fastjson:1.1.58.android'

20.Material-Animations

一句话介绍：一款提供场景转换过渡能力的动画框架

上榜理由：Android动画框架排行榜第二名，9.3k个star数量，与动画框架榜单第一名lottie-android不同的是，Material-Animations提供的是场景切换的动画效果。Android 官网sample中已经提供了部分Transition （转场动画）的展示，作为初学者很难快速拓展到自己项目中，Material-Animations的示例出现为开发者省去了此类麻烦，直接照搬应用到自己的App中吧。

github  https://github.com/lgvalle/Material-Animations

作者：Luis G. Valle

使用：down源码，修改学习



21.tinker

一句话介绍：它是微信官网的Android热补丁解决方案

上榜理由：9.1k个star，微信在用的热补丁方案，心动不如行动

官网地址  http://www.tinkerpatch.com/Docs/intro

github   https://github.com/Tencent/tinker

作者：Tencent



22.ViewPagerIndicator

一句话介绍：一款基于ViewPager的页面指示器开源框架

上榜理由：上古神器，尽管已经五年未更新了，但你仍然可以在淘宝等app中看到它的使用场景，8.9K的star量让它不愠不火的在矗立在榜单里

官网地址 http://viewpagerindicator.com/

github  https://github.com/JakeWharton/ViewPagerIndicator

作者：JakeWharton

使用：

下载地址 https://github.com/JakeWharton/Android-ViewPagerIndicator/zipball/master




23.Android-CleanArchitecture

一句话介绍：一个讲解设计框架的demo

上榜理由：它不是框架，你可以把它当作一本书，它将教会你如何设计简洁的架构，工程里有一个sample app，配合图文讲解，你将对Android客户端的架构有更深一层的认识。8.8k的star数量，证明了它是一本“好书”哟。

github  https://github.com/android10/Android-CleanArchitecture

作者：Fernando Cejas




24..Android-PullToRefresh

一句话介绍：一款为普通视图提供刷新UI的视图框架

上榜理由：8.2K的star数量使它位居刷新类UI框架榜首，强大的兼容能力，该框架支持ListView，GrdiView，WebViewScrollView，ViewPager等众多View增加刷新的能力，如果你有增加上拉加载，下拉加载的需求，你应该考虑它了！

github https://github.com/chrisbanes/Android-PullToRefresh

作者：Chris Banes

使用：

github fork源码，集成到项目中



2525.flexbox-layout

一句话介绍：一款弹性伸缩布局

上榜理由：8.1k个star，前端H5开发者转Android开发的福音，FlexboxLayout作为LinearLayout和RelativeLayout的替代者，值得各位一试，与其一同推出的还有ConstraintLayout。

github  https://github.com/google/flexbox-layout

作者：Google

使用：

dependencies {    compile 'com.google.android:flexbox:0.3.0-alpha3'}

26.AndroidSwipeLayout

一句话介绍：非常强大滑动式布局

上榜理由:滑动删除是国产app常见需求，商品详情的上下滑动需求作为开发者的我们也经常遇到，AndroidSwipeLayout在github上拥有8K个star，证明它经受住了检验，各位值得一试

github https://github.com/daimajia/AndroidSwipeLayout

作者：daimajia

使用：

dependencies {    compile 'com.android.support:recyclerview-v7:21.0.0'    compile 'com.android.support:support-v4:20.+'    compile "com.daimajia.swipelayout:library:1.2.0@aar"}
或下载

AndroidSwipeLayout-v1.1.8.jar



27.realm-java

一句话介绍：Realm是一款移动端数据库框架

上榜理由：核心数据引擎C++打造，比普通的Sqlite型数据库快的多。笔者猜测正是如此，realm以7892个star数让它位于大名鼎鼎的数据库框架GreenDao（7877）之前

官网地址：https://realm.io/cn/

github https://github.com/realm/realm-java

作者：Realm团队

使用：https://realm.io/docs/java/latest/



28.greenDAO

一句话介绍：greenDAO是一款高效、快速的SQLite型数据库

上榜理由：greenDAO的star数量与Realm不相上下，且与EventBus师出同门，也是由greenrobot团队开发维护的，质量有所保证，但若拷问笔者Realm与greenDao两者的优劣性，只能具体到实际使用当中，模拟线上的使用情形，进行高强度测试后才能下判断，故在此不能一言两语说完，深表遗憾

官网地址：http://greenrobot.org/greendao/

github  https://github.com/greenrobot/greenDAO

使用：

buildscript {    repositories {        jcenter()        mavenCentral() // add repository    }    dependencies {        classpath 'com.android.tools.build:gradle:2.3.1'        classpath 'org.greenrobot:greendao-gradle-plugin:3.2.2' // add plugin    }} -----apply plugin: 'com.android.application'apply plugin: 'org.greenrobot.greendao' // apply plugin dependencies {    compile 'org.greenrobot:greendao:3.2.2' // add library}

29.stetho

一句话介绍：一款提供在Chrome开发者工具上调试Android app能力的开源框架

上榜理由：上古时期Android程序员要调试本地数据库，需要进入Android Device Monitor找到/data/data/com.xxx.xxx/databases里面的db文件，导出到PC端，用PC的数据工具查看，现在使用stetho省却了如此的麻烦；如今的Android程序员如果想调试网络请求响应过程中的报文段，需要在请求中加入Log语句，一个信息一个信息打印出来，相当繁琐，现在请使用stetho，省却诸如此类的麻烦把！7.8K个star数，广大Android开发者调试的福音，你值得拥有！

作者：FaceBook

官网地址： http://facebook.github.io/stetho/

github   https://github.com/facebook/stetho

使用：

compile ‘com.facebook.stetho:stetho:1.5.0’



30.BaseRecyclerViewAdapterHelper

一句话介绍：强大、流畅的Recyvlerview通用适配器

上榜理由：如果你是RecyclerView的拥簇者，你一定要体验这款专门服务该view的适配器，7.7K个star，让这个家伙位于github上Android 适配器排行榜第一，还有很多惊喜等你去探寻！

官网地址：http://www.recyclerview.org/

作者：陈宇明以及他的小伙伴

使用：

allprojects {    repositories {        ...        maven { url "https://jitpack.io" }    }}dependencies {        compile 'com.github.CymChad:BaseRecyclerViewAdapterHelper:VERSION_CODE'}

31.AndroidViewAnimations

一句话介绍：一款提供可爱动画集合的框架

上榜理由：正如作者所说，它囊括了开发需求过程中所有的动画效果，集成进了这个简洁可爱的动画框架。7.6K的star数，证明了它在动画框架领域的战斗力，让它仅仅位列lottie-android和Material-Animations两个动画框架霸主之后，屈居第三名

github https://github.com/daimajia/AndroidViewAnimations

作者：daimajia

使用：

dependencies {        compile 'com.android.support:support-compat:25.1.1'        compile 'com.daimajia.easing:library:2.0@aar'        compile 'com.daimajia.androidanimations:library:2.2@aar'}sample：YoYo.with(Techniques.Tada)    .duration(700)    .repeat(5)    .playOn(findViewById(R.id.edit_area));

32.MaterialDrawer


一句话介绍：强大的塑料风格的抽屉框架

上榜理由：7.6K的star数量，作者的持续更新状态，如果你还在犹豫上手SlidingMenu遇到bug没人管的困境，那么你可以入手它作为你的抽屉布局

github  https://github.com/mikepenz/MaterialDrawer

作者：Mike Penz

使用:

compile('com.mikepenz:materialdrawer:5.9.2@aar') {    transitive = true}
new DrawerBuilder().withActivity(this).build();

33.Android-ObservableScrollView

一句话介绍：一款让视图滑动更具有视觉效果的滑动式框架

上榜理由：7.5K的star数量，证明了它曾经的价值，github上提供了12种滑动效果，你可以用它弥补其他框架的不足，提升你的App体验！

github https://github.com/ksoichiro/Android-ObservableScrollView

作者：Soichiro Kashima

使用：

compile com.github.ksoichiro:android-observablescrollview

34.CircleImageView

一句话介绍：圆角ImageView

上榜理由：也许你已经听说过无数种展示圆角图片的方法，但如果你不尝试尝试CircleImageView，那么你的知识库会因为少了它黯然失色，有的时候完成需求是开发者优先考虑的，不同实现方法牵扯到的性能差异更值得让人深思，如果你有心在图片性能上有所涉猎，那么CircleImageView绝对不会让你败兴而归。最后别忘了记得去看Romain Guy的建议哟。

github https://github.com/hdodenhof/CircleImageView

作者：Henning Dodenhof

使用：

dependencies {    ...    compile 'de.hdodenhof:circleimageview:2.1.0'}
<de.hdodenhof.circleimageview.CircleImageView    xmlns:app="http://schemas.android.com/apk/res-auto"    android:id="@+id/profile_image"    android:layout_width="96dp"    android:layout_height="96dp"    android:src="@drawable/profile"    app:civ_border_width="2dp"    app:civ_border_color="#FF000000"/>

35.logger

一句话介绍：一款让log日志优雅显示的框架

上榜理由：logger作为调试框架，并未给出很强大的能力，它最大的亮点是优雅的输出log信息，并且支持多种格式：线程、Json、Xml、List、Map等，如果你整日沉迷于汪洋大海般的log信息不能自拔，logger就是你的指路明灯！6.6k个star让他位列调试框架第二名，屈居facebook的stetho之后

github https://github.com/orhanobut/logger

作者：Orhan Obut

使用：

compile 'com.orhanobut:logger:2.1.1'
Logger.d(MAP);Logger.d(SET);Logger.d(LIST);Logger.d(ARRAY);Logger.json(JSON_CONTENT);Logger.xml(XML_CONTENT);

36.agera

一句话介绍:一款服务于Android平台的响应式编程框架

上榜理由：google专门推出一套响应式编程框架服务于Android开发者，相比于之响应式编程框架榜首的 RxJava RxAndroid，它更轻量，两者最大的不同点在于agera基于push event、pull data （VS Rx系列 push data）。

github https://github.com/google/agera

作者：Google

使用：

  compile 'com.google.android.agera:agera:1.3.0'
扩展能力

  compile 'com.google.android.agera:content:1.3.0'  compile 'com.google.android.agera:database:1.3.0'  compile 'com.google.android.agera:net:1.3.0'  compile 'com.google.android.agera:rvadapter:1.3.0'  compile 'com.google.android.agera:rvdatabinding:1.3.0'

37.BottmBar

一句话介绍：一款底部导航栏视图框架

上榜理由：底部栏里的王者框架，6.3K的star数量，证明了它的优秀，完全遵循材料设计规范，上手非常方便。如果说缺点，无法设置icon与titile的间距，无法自定义视图的大小等，但这些都可以通过修改源代码解决，笔者献丑也修改了一套符合国内开发者的底部导航框架，即将开源。

github  https://github.com/roughike/BottomBar

作者：Iiro Krankka

使用：

compile 'com.roughike:bottom-bar:2.3.1'

38.Calligraphy

一句话介绍：一款自定义字体框架

上榜理由：如果你还在为一键修改App内所有字体样式而烦恼，6.3K个star的Calligraphy就值得你拥有，它可以同时修改整个整个项目的Textview字体，也可以单独 设置某个Textview的字体，还在等什么，快来试试吧！

github  https://github.com/chrisjenx/Calligraphy

作者：Christopher Jenkins

使用：

dependencies {    compile 'uk.co.chrisjenx:calligraphy:2.3.0'}

39.AndroidSlidingUpPanel

一句话介绍：可拖动的滑动面板视图框架

上榜理由：如果你的项目需要一个可拖拽的滑动式面板（展示某些详情信息，播放音乐，地图信息等），那么推荐你使用它，6.3k个star，来自创业公司umano的作品，证明它是用心推出的杰作

github https://github.com/umano/AndroidSlidingUpPanel

作者：umano

使用：

dependencies {    repositories {        mavenCentral()    }    compile 'com.sothree.slidinguppanel:library:3.3.1'}

40.AppIntro

一句话介绍：一款提供快速制作欢迎页的框架

上榜理由：笔者从未把打算把欢迎页框架纳入排行榜当中，作为国内开发者，ViewPager开发App的欢迎页已经是手到擒来的需求，为何一个开源的欢迎页框架会在github上拥有6.3k个star？也许你会不屑一顾，是的，往往就在不屑一顾的瞬间，机遇就悄悄溜走了。

github https://github.com/apl-devs/AppIntro

作者：Paolo Rotolo

    allprojects {        repositories {            ...            maven { url 'https://jitpack.io' }        }    }    dependencies {            compile 'com.github.apl-devs:appintro:v4.2.0'    }

41.recyclerview-animators

一句话介绍：一款为Recyclerview提供扩展动画能力的框架

上榜理由：有一句老话：如果有天你失去对新事物的兴趣，那就说明你老了。recyclerview已经推出快三年了，还在用listview的人们，是否已经发掘自己渐渐变老；不要灰心，快为你的项目加入recyclerview-animators框架吧，为“自己”加入新鲜的血液和能量！（笔者备注：6.2K个star）

github  https://github.com/wasabeef/recyclerview-animators

作者；https://github.com/wasabeef

使用：

dependencies {  // jCenter  compile 'jp.wasabeef:recyclerview-animators:2.2.6'}

42.dagger

一句话介绍：一款通过依赖注入降低程序间耦合的开发框架

上榜理由：github 上dagger1版本 有6.2k个star ， dagger2版本有7.3k个；由square完成的dagger1版本，到如今google团队接手的dagger2版本，强力开发团队保证了代码在设计上的优越性；如果你想探究Android 领域的设计模式，这也是不错的选择。

官网地址：https://google.github.io/dagger/

github ：https://github.com/google/dagger

作者：google

使用：

dependencies {  compile 'com.google.dagger:dagger:2.x'  annotationProcessor 'com.google.dagger:dagger-compiler:2.x'}If you're using classes in dagger.android you'll also want to include:compile 'com.google.dagger:dagger-android:2.x'compile 'com.google.dagger:dagger-android-support:2.x' annotationProcessor 'com.google.dagger:dagger-android-processor:2.x'

43.Android-Bootstarp

一句话介绍：一款提供在Android应用上实现Bootstrap（web框架）所作出效果的框架

上榜理由：榜单上第二款响应web技术的Android 端框架，还记得第一名是谁吗——flexbox-layout，作为Android开发者，你有必要去了解Web技术了。5.9k个star，证明它不容小觑

github https://github.com/Bearded-Hen/Android-Bootstrap

作者:Bearded-Hen团队

使用：

dependencies {   compile 'com.beardedhen:androidbootstrap:{X.X.X}'}

44.RxBinding

一句话介绍：一款提供UI组件事件响应能力的框架

上榜理由：如果你还未开始RxAndroid 之旅，RxBinding可以作为你的第一站，通过RXBinding，你将理解响应式编程的快乐，让项目里的事件流程更清晰。5.6K个star，RxAndroid作者亲自操刀，快来试用吧！

github  https://github.com/JakeWharton/RxBinding

作者：JakeWharton

Platform bindings:

compile 'com.jakewharton.rxbinding2:rxbinding:2.0.0''support-v4' library bindings:compile 'com.jakewharton.rxbinding2:rxbinding-support-v4:2.0.0''appcompat-v7' library bindings:compile 'com.jakewharton.rxbinding2:rxbinding-appcompat-v7:2.0.0''design' library bindings:compile 'com.jakewharton.rxbinding2:rxbinding-design:2.0.0''recyclerview-v7' library bindings:compile 'com.jakewharton.rxbinding2:rxbinding-recyclerview-v7:2.0.0''leanback-v17' library bindings:compile 'com.jakewharton.rxbinding2:rxbinding-leanback-v17:2.0.0'

45.ListViewAnimations

一句话介绍：一款为ListView提供动展示画效果能力的框架

上榜理由：如果有一天我承认自己老了，我还会排排我的兄弟——ListView，证明我和它一起战斗过。ListViewAnimations的存在就是证明我们这些“老年人”仍有用武之地，也许你有说不出口的难处，无法体会到RecyclerView里动画的快乐，拥有ListViewAnimations，你一样可以骄傲的说，我的孩子（每个item）也有自己的动效啦。（笔者备注 5.6K个star）

github  https://github.com/nhaarman/ListViewAnimations

作者：nhaarman

使用：

repositories {    mavenCentral()}dependencies {    compile 'com.nhaarman.listviewanimations:lib-core:3.1.0@aar'    compile 'com.nhaarman.listviewanimations:lib-manipulation:3.1.0@aar'    compile 'com.nhaarman.listviewanimations:lib-core-slh:3.1.0@aar'}

46.UItimateRecyclerView

一句话介绍：一款提供刷新、加载更多、动画特效等额外能力的RecyclerView框架

上榜理由：榜单上第三次出现RecyclerView的身影，足以证明RecyclerView的优异性，5.5K个star，框架里所提供众多的能力，如果你是个功利开发者，那么此框架会为你节省很多学习时间，它可以完成多item式布局的大多数需求，值得注意的是，这个项目也是在其他项目的思路上二次开发的。

github  https://github.com/cymcsg/UltimateRecyclerView

作者：MarshalChen

使用：

repositories {    jcenter()    }dependencies {    ...    compile 'com.marshalchen.ultimaterecyclerview:library:0.7.2'}

47.uCrop

一句话介绍：一款优雅的图片裁剪框架

上榜理由：5.3K个star，图片编辑模块单独拎出来也是一款优雅的App。

github  https://github.com/Yalantis/uCrop

作者：Yalantis

使用：

allprojects {   repositories {      jcenter()      maven { url "https://jitpack.io" }   }}compile 'com.github.yalantis:ucrop:2.2.1'

48.RxJava-Android-Samples

一句话介绍：一款介绍RxJava使用场景的app

上榜理由：榜单出现的第一个“仅仅为告诉你如何使用另一个项目”的开源项目，它可以说是RxJava的用例，你想得到的想不到的RxJava用法这里都有，这就是为什么它以5.2k个star矗立在这份榜单里的原因。遗憾自己没有创作这么一个受人追捧的demo？赶快动手写个其他的“XX项目用例吧”

github  https://github.com/kaushikgopal/RxJava-Android-Samples

作者：kaushikgopal

使用：

clone到本地慢慢探索吧



4949.AndroidAutoLayout

一句话介绍：一个提供适配能力的框架

上榜理由：5.2K个star，鸿洋老弟的作品，适合小项目的开发团队，拿到设计MM的px像素设计稿是不是很头疼捏？这个框架一键式搞定你的问题，它有很多的不足，但在追求完美适配的路上，你值得探索和了解它！笔者并不推荐把它应用到已经成熟运行的项目中，毕竟市面上已经有太多的适配解决方案了，适配问题就像是个大杂烩，想炒一盘好菜，就得备好各种佐料（适配小方案），当你把各种小佐料用的炉火纯青的时候，你离美食大厨就不远了。

github https://github.com/hongyangAndroid/AndroidAutoLayout

作者：张鸿洋

使用：

dependencies {    compile 'com.zhy:autolayout:1.4.5'}

50.EffectiveAndroidUI

一句话介绍：一款讲解高效展示UI的教学型App

上榜理由：编程新手很难对MVC MVP,MVVM等模式有深刻的理解，如果有一个示例型app，那对初学者会有很大裨益，笔者在遇到它时也是相见恨晚。4.8K个star，证明了它经受了广大开发者的考验与审视，其中Effective UI的编程思想更是与Android官方课程里的Effective UI课程不谋而合，并且，此项目还包含了fragment、dagger、主题样式、Butterknife等众多小知识点，作为编程初学者的学习用例再适合不过了

github  https://github.com/pedrovgs/EffectiveAndroidUI

作者：Pedro Vicente

使用：

clone项目到本地




51.Luban

一句话介绍：最接近微信的图片压缩框架

上榜理由：好的思路总是可以让你大放异彩，Luban仅以图片压缩单一功能，俘获了4.8K个star，证明了它在图片压缩上的造诣，它可能不是最优秀的，但它是让你我最接近伟大的项目

github  https://github.com/Curzibn/Luban

作者：Curzibn

使用：

compile 'top.zibin:Luban:1.1.1'

52.DroidPlugin

一句话介绍：一款热门的插件化开发框架
上榜理由：4.8K个star，插件化框架榜单第一名，，360团队出品，框架质量有保证，有成功案例——360手机助手，并且持续维护着
github https://github.com/DroidPluginTeam/DroidPlugin/blob/master/readme_cn.md
作者：Andy Zhang
使用:
clone项目到本地



5353.otto

一句话介绍:一款老旧且强大的事件总线框架
上榜理由：4.8K个star，是square团队早先推出的事件响应型框架，淘宝app的事件驱动也是基于此框架封装的，如今square已经建议开发者采用RxJava RxAndroid来代替otto了。但otto仍有与EventBus横向对比的价值，纵向来说，otto与square自家开发的Rx系列框架的差异同样值得开发者们去探究。
github https://github.com/square/otto
作者：square
使用：

repositories {    mavenCentral()    maven { url "https://oss.sonatype.org/content/repositories/snapshots/" }}compile 'com.michaelpardo:activeandroid:3.1.0-SNAPSHOT'

54.u2020

一句话介绍：一款提供Dagger的高级教学示例的app（额，名字是有点绕）
上榜理由：4.7K个star，JakeWharton牵头开发的教学类app，教你使用Dagger在其他高级框架的用法，它展示了Dagger与ButterKnife、Retrofit、Moshi、Picasso、Okhttp、RxJava、Timber、Madge、LeakCanar等众多优秀框架结合起来的高级用法，你也可以借鉴到自己的项目当中
github  https://github.com/JakeWharton/u2020
作者：JakeWharton



55.buck

一句话介绍：buck是一个快速构建系统
上榜理由：facebook+google出身的作者，对构建代码的出色理解，加上大型团队的维护，以及增量更新时的快速高效，让buck成为了微信Android团队构建项目的首选，构建大型项目时，它比gradle更快，然而中小公司并不适合此框架，但作为立志在框架设计领域有一番作为的人们，欢迎来一探究竟
官网地址：https://buckbuild.com/
github  https://github.com/facebook/buck
作者：facebook
使用：
linux or mac system  +docs




56.PermissionsDispatcher

一句话介绍：一款基于注解的提供解决运行时危险权限方案的框架
上榜理由：自Android6.0 Google提出危险权限一词起，用户安全性被提到一定的高度，一些运行时对用户较为危险的权限将不再自动被开发者获取，需要经过用户批准，开发者才可以继续使用该权限，如果你曾经被权限问题搞的抓耳挠腮，建议你试试这个框架，它足够解决你的问题
官网地址：https://hotchemi.github.io/PermissionsDispatcher/
github https://github.com/hotchemi/PermissionsDispatcher
作者：Shintaro Katafuchi
使用：

dependencies {  compile('com.github.hotchemi:permissionsdispatcher:${latest.version}') {      exclude module: "support-v13"  }  annotationProcessor 'com.github.hotchemi:permissionsdispatcher-processor:${latest.version}'}repositories {  jcenter()  maven { url 'http://oss.jfrog.org/artifactory/oss-snapshot-local/' }}

57.android-gif-drawable

一句话介绍:一款提供展示GIF动画能力的视图框架

上榜理由：据我所查国内著名App——知乎使用了android-gif-drawable，因此证明了它的存在价值，尽管在榜单第十一位介绍了lottie-android直接应用AE动画的示例，但AE设计师不是每个公司都配备的，GIF的存在，就必然存在了展示GIF的需要，它值得你拥有！

github https://github.com/koral--/android-gif-drawable

作者：Karol Wrótniak

使用：

repositories {    mavenCentral()    maven { url "https://oss.sonatype.org/content/repositories/snapshots" }}dependencies {    compile 'pl.droidsonroids.gif:android-gif-drawable:1.2.+'}

58.Apktool

一句话介绍：一款反编译apk的工具

上榜理由：开源的反编译工具，对于志在了解apk逆向破解的诸位，值得拥有，4.5k个star，逆向破解apk神器！

github  https://github.com/iBotPeaches/Apktool

官网地址：https://ibotpeaches.github.io/Apktool/

作者：Connor Tumbleson



59.dynamic-load-apk

一句话介绍：插件化开发框架

上榜理由：4.5k个star，位于插件化开发框架第二名（第一名来自360团队），全面的文档介绍让你很快就能上手插件化开发，如果你喜欢大段文字讲解，那么这个项目一定适合你

github：https://github.com/singwhatiwanna/dynamic-load-apk

作者：singwhatiwanna

使用：

github上的文档配合作者博客更配哟



60.atlas

一句话介绍：淘宝推出的组件化开发框架

上榜理由：淘宝团队所出的精品，atlas框架提供了解耦、组件、动态的开发能力，4.5k个star让他位列组件化开发框架第一名

github https://github.com/alibaba/atlas

作者：alibaba
