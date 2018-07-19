# QT进阶之路

<a name="目录"></a>

# 目录

<a href="#w1">第1节</a>

<a href="#w2">第2节</a>

<a href="#w3">第3节</a>

<a href="#w4">第4节</a>

<a href="#w5">第5节</a>

<a href="#w6">第6节</a>

<a href="#w7">第7节</a>

<a href="#w8">第8节</a>

<a href="#w9">第9节</a>

<a href="#w10">第10节</a>

<a href="#w11">第11节</a>

<a href="#w12">第12节</a>

<a href="#w13">第13节</a>


-------

### 
<a name="w1"></a>

-------
# 第1节 关于QT

<a href="#目录">回到目录</a>

> 什么是Qt ？
> - Qt是一个针对桌面、嵌入式、移动设备的一个跨平台的应用程序开发框架，支持的平台包括Linux、OS X、Windows、VxWorks、QNX、Android、iOS、BlackBerry(黑莓)、Sailfish OS（旗鱼操作系统）等。
Qt 1991年由Trolltech-奇趣科技（成立于1994年）开发，2008年，Trolltech被Nokia收购，2012年，Qt被Digia收购。
> - Qt是基于C++编写的框架，它既可以开发GUI程序，也可用于开发非GUI程序，比如控制台工具和服务器。预处理器，MOC（全称：Meta-Object Compiler-元对象编译器）用于扩展C++，如：信号和槽的特性。在编译之前，先使用MOC分析Qt扩展的C++源文件（检测是否包含Q_OBJECT宏），然后生成符合C++标准的源文件（新文件名将会由moc_加上原文件名构成）。因此框架本身和应用程序/库使用它能被任何符合标准C++的编译器（像Clang、GCC、 ICC、MinGW 和MSVC）所编译。
> 平台支持：
> - MS/Windows - 95、98、NT4.0、ME、2000、XP 、Vista、Win7、win8、win2008、win10
> - Unix/X11-Linux、SunSolaris、HP-UX、CompaqTru64 UNIX、IBMAIX、SGI IRIX、FreeBSD、BSD/OS和其它很多X11平台
> - Macintosh -Mac OS X
> - Symbian、Symbian^3、Symbian Anna、Symbian Belle、MeeGo

> 优点：
> - 优良的跨平台特性： 
>    - Qt支持下列操作系统: Microsoft Windows 95/98， Microsoft Windows NT， Linux， Solaris， SunOS， HP-UX， Digital UNIX (OSF/1， Tru64)， Irix， FreeBSD， BSD/OS， SCO， AIX， OS390，QNX 等等。
> - 面向对象 
>    - Qt 的良好封装机制使得 Qt 的模块化程度非常高，可重用性较好，对于用户开发来说是非常 方便的。 Qt 提供了一种称为 signals/slots 的安全类型来替代 callback，这使得各个元件 之间的协同工作变得十分简单。
> - 丰富的 API 
>    - Qt包括多达250个以上的C++类，还替供基于模板的collections、serialization、 file、I/O device、 directory management、date/time 类。甚至还包括正则表达式的处理功能。
> - 支持 2D/3D 图形渲染，支持 OpenGL
> - 大量的开发文档
> - XML 支持
> Qt Creator
> - 简介
>    - 在发布 Qt 4.6 的同时，作为 Qt 开发跨平台 IDE 的Qt Creator也发布了更新版本。Qt Creator 1.3 和 Qt 4.6共同构成的 Qt SDK，包含了开发跨平台应用程序所需的全部功能。
>    - Qt Creator是一个用于Qt开发的轻量级跨平台集成开发环境。Qt Creator可带来两大关键益处：提供首个专为支持跨平台开发而设计的集成开发环境 (IDE)，并确保首次接触Qt框架的开发人员能迅速上手和操作。即使不开发Qt应用程序，Qt Creator也是一个简单易用且功能强大的IDE。
>    - Qt Creator 包括项目生成向导、高级的 C++ 代码编辑器、浏览文件及类的工具、集成了 Qt Designer、Qt Assistant、Qt Linguist、图形化的 GDB 调试前端，集成 qmake 构建工具等。
> - 功能和优势
>    - QtCreator 主要是为了帮助新 Qt 用户更快速入门并运行项目，还可提高有经验的 Qt 开发人员的工作效率。
>    - 使用强大的 C++ 代码编辑器可快速编写代码
>    - 语法标识和代码完成功能输入时进行静态代码检验以及提示样式上下文相关的帮助代码折叠括号匹配和括号选择模式高级编辑功能
>    - 使用浏览工具管理源代码
>    - 集成了领先的版本控制软件，包括 Git、Perforce 和 Subversion开放式文件，无须知晓确切的名称或位置搜索类和文件跨不同位置或文件沿用符号在头文件和源文件，或在声明和定义之间切换
>    - 为Qt跨平台开发人员的需求而量身定制
>    - 集成了特定于 Qt 的功能，如信号与槽 (Signals & Slots)图示调试器， 对 Qt 类结构可一目了然集成了 Qt Designer 可视化布局和格式构建器只需单击一下就可生成和运行 Qt 项目

> Qt Designer
> - Qt Designer被称为Qt设计师，用于设计和构建图形用户界面（Qt Widgets）。你可以组合和自定义窗口或对话框（所见即所得），并使用不同的风格和分辨率进行测试。用Qt Designer创建的窗口部件和表格无缝集成编程代码，采用Qt信号和槽机制，这样就可以轻松地分配图形元素的行为。在Qt设计师中设置的所有属性可以动态地在代码中进行更改。此外，类似插件推广和自定义插件功能，可以使用自己的组件来使用Qt Designer。
> - 注意：你也可以选择使用Qt Quick来设计用户界面，而不是Qt Widgets。这样更容易写各种各样的应用。它可以完全定制外观，触摸反应的元素，流畅的动画过渡，支持OpenGL图形加速功能。如果刚接触Qt Designer，可以看看Qt设计师文档。有关如何使用Qt设计师，请参阅Qt设计师快速入门。

> Qt Linguist
> - 简介
>    - Qt Linguist被称为Qt语言家。主要任务是读取翻译文件、为翻译人员提供友好的翻译界面，是用于界面国际化的重要工具。它能帮助你很容易读懂C++语言。
> - 使用方式
>    - lupdate可以把.h、.cpp、.ui中需要翻译的字符串提取出来形成.ts文件，然后用linguist翻译。用lerealse生成.qm。
>    - 翻译一个含有tr()调用的Qt应用程序需要以下三步： 
>       - 运行ludate，从应用程序的源代码中提取所有用户可见的字符串。 
>       - 使用Qt Linguist翻译该应用程序。 
>       - 运行lrelease，生成二进制.qm文件，应用程序可以使用QTranslator加载这个文件。 
如果开发工程中出现翻译改动，可以多次执行此过程！

> Qt Assistant
> - Qt Assistant被称为Qt助手，是Qt自带的一款可定制、可重新发行的帮助文件浏览器。它支持HTML文件，用户可以利用其定制自己的功能强大的帮助文档浏览器。
