---
layout : post
title : "个性化控件(View)篇(ListView)"
category : 开源项目
duoshuo: true
date : 2015-07-24
tags : [Project , Android ]
SyntaxHihglighter: true
shTheme: shThemeMidnight # shThemeDefault  shThemeDjango  shThemeEclipse  shThemeEmacs  shThemeFadeToGrey  shThemeMidnight  shThemeRDark
---

Android优秀开源项目汇总——个性化控件(View)篇(ListView)介绍

android-Ultra-Pull-to-Refresh  
下拉刷新，第一个项目已经停止维护了，并且使用起来相对复杂，定制性也差。这个是替代和改良方案。这个继承于ViewGroup可以包含任何View。功能甚至比SwipeRefreshLayout强大。使用起来非常简单。良好的设计，如果你想定制自己的UI样式，非常简单，就像给ListView加一个Header View那么简单。  
支持 `API LEVEL >= 8`  
项目地址：https://github.com/liaohuqiu/android-Ultra-Pull-To-Refresh  
Demo地址：https://github.com/liaohuqiu/android-Ultra-Pull-To-Refresh/blob/master/ptr-demo/target/ultra-ptr-demo.apk?raw=true  
<div>  
  <img src='http://srain-github.qiniudn.com/ultra-ptr/contains-all-of-views.gif' width="150px"/>  
  <img src='http://srain-github.qiniudn.com/ultra-ptr/release-to-refresh.gif' width="150px"/>  
  <img src='http://srain-github.qiniudn.com/ultra-ptr/auto-refresh.gif' width="150px"/>  
  <img src='http://srain-github.qiniudn.com/ultra-ptr/store-house-string-array.gif' width="150px"/>  
</div>

<!-- more -->

---

**android-pulltorefresh**  
一个强大的拉动刷新开源项目，支持各种控件下拉刷新，ListView、ViewPager、WevView、ExpandableListView、GridView、ScrollView、Horizontal  ScrollView、Fragment上下左右拉动刷新，比下面johannilsson那个只支持ListView的强大的多。并且它实现的下拉刷新ListView在item不足一屏情况下也不会显示刷新提示，体验更好。  
项目地址：https://github.com/chrisbanes/Android-PullToRefresh  
Demo地址：https://github.com/Trinea/TrineaDownload/blob/master/pull-to-refreshview-demo.apk?raw=true  
APP示例：新浪微博各个页面  

**android-pulltorefresh-listview**  
下拉刷新ListView，这个被很多人使用的项目实际有不少bug，推荐使用上面的android-pulltorefresh  
项目地址：https://github.com/johannilsson/android-pulltorefresh  
Demo地址：https://github.com/Trinea/TrineaDownload/blob/master/pull-to-refresh-listview-demo.apk?raw=true  

**DropDownListView**  
下拉刷新及滑动到底部加载更多ListView  
项目地址：https://github.com/Trinea/AndroidCommon  
Demo地址：https://play.google.com/store/apps/details?id=cn.trinea.android.demo  
文档介绍：http://www.trinea.cn/android/dropdown-to-refresh-and-bottom-load-more-listview/  

**DragSortListView**  
拖动排序的ListView，同时支持ListView滑动item删除，各个Item高度不一、单选、复选、CursorAdapter做为适配器、拖动背景变化等  
项目地址：https://github.com/bauerca/drag-sort-listview  
Demo地址：https://play.google.com/store/apps/details?id=com.mobeta.android.demodslv  
APP示例：Wordpress Android  

**SwipeListView**  
支持定义ListView左右滑动事件，支持左右滑动位移，支持定义动画时间  
项目地址：https://github.com/47deg/android-swipelistview  
Demo地址：https://play.google.com/store/apps/details?id=com.fortysevendeg.android.swipelistview  
APP示例：微信  

**Android-SwipeToDismiss**  
滑动Item消失ListView，支持3.0以下版本见：https://github.com/JakeWharton/SwipeToDismissNOA  
项目地址：https://github.com/romannurik/Android-SwipeToDismiss  
Demo地址：https://github.com/JakeWharton/SwipeToDismissNOA/SwipeToDismissNOA.apk/qr_code  

**PinnedHeaderExpandableListView**  
首先它是一个ExpandableListView，但是它的头部可以固定，其次，在它的上面还有一个头部可以来回伸缩  
项目地址：https://github.com/singwhatiwanna/PinnedHeaderExpandableListView  
APP示例：百度手机卫士垃圾清理界面  
![Renderings](https://camo.githubusercontent.com/fa7f516b0b6e2921007a17cbc359b3f661f32226/687474703a2f2f696d672e626c6f672e6373646e2e6e65742f32303134303531313135313534363834333f77617465726d61726b2f322f746578742f6148523063446f764c324a736232637559334e6b626935755a58517663326c755a33646f5958527064324675626d453d2f666f6e742f3561364c354c32542f666f6e7473697a652f3430302f66696c6c2f49304a42516b46434d413d3d2f646973736f6c76652f37302f677261766974792f536f75746845617374)  


**StickyListHeaders**  
GroupName滑动到顶端时会固定不动直到另外一个GroupName到达顶端的ExpandListView，支持快速滑动，支持Android2.3及以上  
项目地址：https://github.com/emilsjolander/StickyListHeaders  
APP示例：Android 4.0联系人  
![Renderings](https://raw.github.com/emilsjolander/StickyListHeaders/master/demo.gif)  
  

**pinned-section-listview**  
GroupName滑动到顶端时会固定不动直到另外一个GroupName到达顶端的ExpandListView  
项目地址：https://github.com/beworker/pinned-section-listview  
![Renderings](https://raw.github.com/beworker/pinned-section-listview/master/screen1.png)  

**PinnedHeaderListView**  
GroupName滑动到顶端时会固定不动直到另外一个GroupName到达顶端的ExpandListView  
项目地址：https://github.com/JimiSmith/PinnedHeaderListView  

**QuickReturn**  
ListView/ScrollView的header或footer，当向下滚动时消失，向上滚动时出现  
项目地址：https://github.com/lawloretienne/QuickReturn  
Demo地址：https://play.google.com/store/apps/details?id=com.etiennelawlor.quickreturn  

**QuickReturnHeader**  
ListView/ScrollView的header或footer，当向下滚动时消失，向上滚动时出现  
项目地址：https://github.com/ManuelPeinado/QuickReturnHeader  
Demo地址：https://github.com/Trinea/TrineaDownload/blob/master/quick-return-header-demo.apk?raw=true  
APP示例：google plus  

**IndexableListView**  
ListView右侧会显示item首字母快捷索引，点击可快速滑动到某个item  
项目地址：https://github.com/woozzu/IndexableListView  
Demo地址：https://github.com/Trinea/TrineaDownload/blob/master/indexable-listview.apk?raw=true  
APP示例：微信通讯录、小米联系人  

**CustomFastScrollView**  
ListView快速滑动，同时屏幕中间PopupWindows显示滑动到的item内容或首字母  
项目地址：https://github.com/nolanlawson/CustomFastScrollViewDemo  

**Android-ScrollBarPanel**  
ListView滑动时固定的Panel指示显示在scrollbar旁边  
项目地址：https://github.com/rno/Android-ScrollBarPanel  

**SlideExpandableListView**  
用户点击listView item滑出固定区域，其他item的区域收缩  
项目地址：https://github.com/tjerkw/Android-SlideExpandableListView  
Demo地址：https://github.com/Trinea/TrineaDownload/blob/master/slide-expandable-listView-demo.apk?raw=true  

**JazzyListView**  
ListView及GridView item以特殊动画效果进入屏幕，效果包括grow、cards、curl、wave、flip、fly等等  
项目地址：https://github.com/twotoasters/JazzyListView  
Demo地址：https://play.google.com/store/apps/details?id=com.twotoasters.jazzylistview.sample  
在线演示：http://lab.hakim.se/scroll-effects/  

**ListViewAnimations**  
带Item显示动画的ListView，动画包括底部飞入、其他方向斜飞入、下层飞入、渐变消失、滑动删除等  
项目地址：https://github.com/nhaarman/ListViewAnimations  
Demo地址：https://play.google.com/store/apps/details?id=com.haarman.listviewanimations  
APP示例：Google plus、Google Now卡片式进入、小米系统中应用商店、联系人、游戏中心、音乐、文件管理器的ListView、Ultimate、Light Flow Lite、TreinVerkeer、Running Coach、Pearl Jam Lyrics、Calorie Chart、Car Hire、Super BART、DK FlashCards、Counter Plus、Voorlees Verhaaltjes 2.0  

**DevsmartLib-Android**  
横向ListView  
项目地址：https://github.com/dinocore1/DevsmartLib-Android  
Demo地址：https://github.com/Trinea/TrineaDownload/blob/master/horizontal-listview-demo.apk?raw=true  

**TwoWayView**  
横向ListView的效果，继承自AdapterView  
项目地址：https://github.com/lucasr/twoway-view  

**HorizontalVariableListView**  
支持Item宽度不一致的ListView  
项目地址：https://github.com/sephiroth74/HorizontalVariableListView  

**LinearListView**  
用LinearLayout实现的ListView，可解决多个ListView并存等问题。目前自己也有需要，等亲自尝试过后会再具体介绍  
项目地址：https://github.com/frankiesardo/LinearListView  

**MultiChoiceAdapter**  
支持多选的ListView Adapter  
项目地址：https://github.com/ManuelPeinado/MultiChoiceAdapter  
Demo地址：https://play.google.com/store/apps/details?id=com.manuelpeinado.multichoiceadapter.demo  

**EnhancedListView**  
支持横向滑动删除列表项以及撤销删除的ListView，该项目的前身是[SwipeToDismissUndoList](https://github.com/timroes/SwipeToDismissUndoList)  
项目地址：https://github.com/timroes/EnhancedListView  
Demo地址：https://play.google.com/store/apps/details?id=de.timroes.android.listviewdemo&rdid=de.timroes.android.listviewdemo  

**ListBuddies**  
自动滚动的双列ListView ，两个ListView滚动速度不一致，有视差效果  
项目地址：https://github.com/jpardogo/ListBuddies  
Demo地址：https://play.google.com/store/apps/details?id=com.jpardogo.android.listbuddies  

**SwipeMenuListView**  
针对ListView item的侧滑菜单  
项目地址：https://github.com/baoyongzhang/SwipeMenuListView  
APP示例：手机QQV5.0  
![Renderings](https://raw.githubusercontent.com/baoyongzhang/SwipeMenuListView/master/demo.gif)  


**PagingListView**  
分页加载的ListView。当滑动到ListView底部最后一个元素时，显示一个进度行，然后加载下一页数据，并显示。  
项目地址：https://github.com/nicolasjafelle/PagingListView  

**PullZoomView**  
支持下拉时HeaderView缩放的ListView、ScrollView  
项目地址：https://github.com/Frank-Zhu/PullZoomView  
![Renderings](https://raw.githubusercontent.com/Frank-Zhu/PullZoomView/master/art/pull-to-zoom.gif)  

**PullToZoomInListView**  
滑动ListView时使其HeaderView跟随滑动缩放  
项目地址：https://github.com/matrixxun/PullToZoomInListView  
![Renderings](https://github.com/matrixxun/PullToZoomInListView/raw/master/art/pull-to-zoom.gif)  

**CalendarListview**  
实现每个月一行日历效果的ListView  
项目地址：https://github.com/traex/CalendarListview  
![Renderings](https://github.com/traex/CalendarListview/raw/master/demo.gif)  

**sticky-headers-recyclerview**  
GroupName滑动到顶端时会固定不动直到另外一个GroupName到达顶端的ListView，采用support-v7中的RecyclerView实现  
项目地址：https://github.com/timehop/sticky-headers-recyclerview  

**PullSeparateListView**  
到达顶部或底部继续拉动时，实现Item间的相互分离，两种模式：(1) 全部分离的模式，即屏幕内所有Item都会分离 (2)部分分离模式，以点击位置为分界点，部分item分离  
项目地址：https://github.com/chiemy/PullSeparateListView  
![Renderings](https://github.com/chiemy/PullSeparateListView/raw/master/capture.gif)  

**ExpandableLayout**  
Header 和 Content Item 都可以展开的 ExpandableListview  
项目地址：https://github.com/traex/ExpandableLayout  

**PagedHeadListView**  
支持paginated header以及material page indicator的ListView.  
项目地址：https://github.com/JorgeCastilloPrz/PagedHeadListView  
![Renderings](https://raw.githubusercontent.com/JorgeCastilloPrz/PagedHeadListView/master/app/src/main/res/raw/preview1.gif)  
  

**CustomSwipeListView**  
支持左滑弹出自定义菜单，右滑删除且允许撤销，同时可以自定义滑动动画时间和滑动触发事件的时机等。   
项目地址：https://github.com/xyczero/Android-CustomSwipeListView   
Demo地址：[Download here](http://7u2jsw.com1.z0.glb.clouddn.com/githubCustomSwipeListView.apk)   

**Pull-to-Refresh.Rentals-Android**  
提供一个简单可以自定义的下拉刷新实现，[Yalantis](http://yalantis.com/) 出品。  
项目地址：https://github.com/Yalantis/Pull-to-Refresh.Rentals-Android  


