---
layout : post
title : "SegmentFault中关于decltype返回数组指针"
category : SegmentFault
duoshuo: true
date : 2015-07-13
tags : [SegmentFault]
SyntaxHihglighter: true
shTheme: shThemeMidnight # shThemeDefault  shThemeDjango  shThemeEclipse  shThemeEmacs  shThemeFadeToGrey  shThemeMidnight  shThemeRDark
---

>int a[2] = { 2, 4 };  
>using type1 = int[2];  
>using type2 = int(*)[2];  
>using type3 = int(&)[2];  

>decltype(a)获得是数组类型

<!-- more -->

decltype(a) 的类型是上述```type1```,而```decltype(a) * p2 = a```,相当于```type2 p2 = a```

即等号左边是```int(*)[2]```,等号右边是```int[2]```,**显然不能划等号**

<pre class="brush: c; ">
	cout << *(*p2 + 1) << endl;//4
</pre>

```decltype(a) * p2 ```<==>``` type1 *p2```

所以，```*p2```的类型就是```type1```,a的类型也是```type1```,若有 ```decltype(a) * p2 = &a;``` 则 ```*p2``` 就是``` a.```因此,```*(*p2 + 1) <==> *(a + 1) <==> a[1] <==> 4```

**如下测试：**

<pre class="brush: c; ">
	cout << p1 << endl;//00488860
	cout << *p2 + 1 << endl;//00488864
	cout << p2 << endl;//00488860
	cout << &a << endl;//00488860
	cout << &a + 1 << endl;//00488868
</pre>

**画图解释：**

 __________ __________ __________ __________  
|_____2 ___|____4_____|_____x____|_____x____|  
|0x00488860|0x00488864|0x00488868|0x00488872|  
|<--------&a--------->|<--------&a+1------->|  
|<----p--->|<--p+1--->|  

a的类型是```int[2]```,那么，```&a```的类型是```int(&)[2],即type3```，而```int *p = a```，这个 p 的类型是```int*```。而``` *p2 + 1 <==> a + 1 <==> p + 1```。三种类型如上图所示范围。













