---
layout : post
title : "个性化控件(View)篇(GridView)"
category : 开源项目
duoshuo: true
date : 2015-07-24
tags : [Project , Android ]
SyntaxHihglighter: true
shTheme: shThemeMidnight # shThemeDefault  shThemeDjango  shThemeEclipse  shThemeEmacs  shThemeFadeToGrey  shThemeMidnight  shThemeRDark
---

Android优秀开源项目汇总——个性化控件(View)篇(GridView)介绍

**GridView with Header and Footer**  
和`ListView`一样带头部和底部的`GridView`，用法和`ListView`一样  
项目地址：https://github.com/liaohuqiu/android-GridViewWithHeaderAndFooter  

<!-- more -->

---

**StaggeredGridView**  
允许非对齐行的GridView，类似Pinterest的瀑布流，并且跟ListView一样自带View缓存，继承自ViewGroup  
项目地址：https://github.com/maurycyw/StaggeredGridView  
Demo地址：https://github.com/Trinea/TrineaDownload/blob/master/staggered-gridview-demo.apk?raw=true  
APP示例：Pinterest等  

**AndroidStaggeredGrid**  
允许非对齐行的GridView，类似Pinterest的瀑布流，继承自AbsListView  
项目地址：https://github.com/etsy/AndroidStaggeredGrid  
APP示例：Pinterest等  

**PinterestLikeAdapterView**  
允许非对齐行的GridView，类似Pinterest的瀑布流，允许下拉刷新  
项目地址：https://github.com/GDG-Korea/PinterestLikeAdapterView  
APP示例：Pinterest等  

**DraggableGridView**  
Item可拖动交换位置的GridView，实际是自己继承ViewGroup实现，类似桌面的单屏效果，可屏幕自动上下滚动进行Item移动交换，多屏效果见下面PagedDragDropGrid  
项目地址：https://github.com/thquinn/DraggableGridView  
Demo地址：https://github.com/thquinn/DraggableGridView/blob/master/bin/DraggableGridViewSample.apk?raw=true  

**StickyGridHeaders**  
GroupName滑动到顶端时会固定不动直到另外一个GroupName到达顶端的GridView  
项目地址：https://github.com/TonicArtos/StickyGridHeaders  

**PagedDragDropGrid**  
Item可拖动交换位置、拖动删除的自定义控件，实际是自己继承ViewGroup实现，类似桌面的多屏效果，可拖动到屏幕边缘，屏幕自动左右滚动进行Item移动交换，可拖动进行删除，单屏效果见上面DraggableGridView  
项目地址：https://github.com/mrKlar/PagedDragDropGrid  
在线演示：http://youtu.be/FYTSRfthSuQ  

**Android-DraggableGridViewPager**  
Item可拖动交换位置的GridView，实际是自己继承ViewGroup实现，类似桌面的多屏效果，可屏幕自动左右滚动进行Item移动交换，单屏效果见上面DraggableGridView  
项目地址：https://github.com/zzhouj/Android-DraggableGridViewPager  
Demo地址：https://github.com/Trinea/trinea-download/blob/master/draggable-grid-viewpager-demo.apk?raw=true  

**TwoWayGridView**  
可横向滚动的GridView  
项目地址：https://github.com/jess-anders/two-way-gridview  

**PagingGridView**  
分页加载的GridView。当滑动到GridView底部最后一个行时，显示一个进度行，然后加载下一页数据，并显示。  
项目地址：https://github.com/nicolasjafelle/PagingGridView  

**AsymmetricGridView**  
一个支持跨行和跨列可变Item大小的GridView  
项目地址：https://github.com/felipecsl/AsymmetricGridView  
Demo地址：https://play.google.com/store/apps/details?id=com.felipecsl.asymmetricgridview.app  





