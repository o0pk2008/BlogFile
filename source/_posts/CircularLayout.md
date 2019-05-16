---
title: 拓扑圆形布局算法
date: 2019-05-16 15:25:09
tags: 算法
categories: ThreeJS
---
![最终效果](img.jpg)
{% codeblock 拓扑圆形布局算法 %}
for (var i = 节点数; i > 0; i--) {
    let centerX = 0; //中心点X
    let centerZ = 0; //中心点Y
    let radius = 1.3; //半径
    let x = centerX + (radius * Math.cos(Math.PI * 2 / 节点数 * i));
    let z = centerZ + (radius * Math.sin(Math.PI * 2 / 节点数 * i));
    console.log("x:", x, "z:", z);
}
{% endcodeblock %}