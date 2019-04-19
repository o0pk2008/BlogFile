---
title: c++ fopen 编译报错解决
date: 2019-04-19 17:12:06
tags: C++
categories: C++
---
1.fopen改成了fopen_s后会产生更多错误比较麻烦；
2.可以在程序前面加上 _CRT_SECURE_NO_WARNINGS 的宏定义，或设置 项目（Project） -> 属性（Properties） -> C/C++ -> 预处理器（Preprocessor） -> 预处理器定中添加 _CRT_SECURE_NO_WARNINGS 这个预定义；
{% codeblock 宏定义 %}
#define _CRT_SECURE_NO_WARNINGS
{% endcodeblock %}