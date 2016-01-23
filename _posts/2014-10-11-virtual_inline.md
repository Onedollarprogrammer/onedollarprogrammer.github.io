---
layout : post
title : "虚函数为什么不能是内联的"
category : C++
duoshuo: true
date : 2014-10-11
tags : [C++]
SyntaxHihglighter: true
shTheme: shThemeMidnight # shThemeDefault  shThemeDjango  shThemeEclipse  shThemeEmacs  shThemeFadeToGrey  shThemeMidnight  shThemeRDark
---
**在C++面向对象过程中，虚函数为什么不能是内联的？**

<!-- more -->

在实际运行中，虚函数所需的代价与内联函数有关，但是实际上虚函数是不能内联的。首先应该区别**内联** 与 **虚**的区别。

**内联**是指**在编译期间用被调用的函数体本身来代替函数调用的指令。**

**虚**是指**直到运行时才能知道要调用的是哪一个函数。**

倘若编译器在某个函数的调用点不知道具体是哪个函数被调用，就能知道为什么它不会内联该函数的调用。事实上是**放弃了使用内联函数**。
当通过对象调用虚函数时，它可以被内联，但是大多数虚函数是通过对象的指针或引用来被调用的，这种调用不能被内联。因为这种调用时标准的调用方式，所以
虚函数实际上不能被内联。
