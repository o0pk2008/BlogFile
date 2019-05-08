---
title: UE4_开启WebGL与卡死问题解决
date: 2019-04-25 14:54:04
tags: UE4
categories: UE4
---
其实UE4开启WebGL很简单只需要添加已下代码：
WebBrowserSingleton.cpp
{% codeblock WebGL %}
//Ning+ 20190430
BrowserSettings.plugins = STATE_ENABLED;
BrowserSettings.webgl = STATE_ENABLED;
{% endcodeblock %}

CEFBrowserApp.cpp
{% codeblock WebGL %}
//Ning+ 20190430
CommandLine->AppendSwitch("enable-gpu");
CommandLine->AppendSwitch("enable-gpu-compositing");
{% endcodeblock %}

性能优化,具体看自己需要添加
{% codeblock WebGL %}
//Ning+ 20190430
command_line->AppendSwitch("enable-native-gpu-memory-buffers");
command_line->AppendSwitch("enable-one-copy");
command_line->AppendSwitch("enable-viewport");
command_line->AppendSwitch("no-proxy-server");
command_line->AppendSwitch("no-sandbox");
command_line->AppendSwitchWithValue("num-raster-threads", "4");
command_line->AppendSwitch("renderer");
{% endcodeblock %}

网上的教程通常就到这里，当你完成这些步骤后确实可以加载WebGL，但是不到几分钟就会卡住；
接下来关键点来了，如何解决这个BUG？
方法就是利用VS的调试工具，当UE4卡住时候查看堆栈，定位到CEF消息循环事件，将此屏蔽，然后自定义消息循环事件，利用UE4的Tick事件驱动；这样才算是真正打开了UE4的WebGL功能；