---
title: 自己写的一个ThreeJS的粒子发射器
date: 2019-05-16 15:48:03
tags: 经验积累
categories: ThreeJS
---
因为最近项目需要基于ThreeJS做很多粒子特效，感觉UE4的粒子发射器做这种效果会比较方便，所以就以UE4粒子发射器的思路手写了一个ThreeJS的粒子发射器，思路很简单：
1.生产粒子；
2.管理粒子；
3.粒子运动；
4.粒子发射；
后期还可以根据需要扩展很多其他的功能效果；
代码如下：
{% codeblock ThreeJsParticleSystem By_Ning+ %}
//生产粒子 Ning+
function GreatSprite() {
    var textureLoader = new THREE.TextureLoader();
    var mapC = textureLoader.load("img/LineSprite4.png");
    var materialC = new THREE.SpriteMaterial({
        map: mapC,
        transparent: true,
        opacity: 0, //初始化0-1
        alphaTest: 0.2
        // color: 0xffffff,
        // fog: true
    });
    var sprite = new THREE.Sprite(materialC);
    sprite.scale.set(0.8, 0.8, 1);
    return (sprite);
}

//管理粒子 Ning+
var SpriteGroup = new THREE.Group();
function GreatSpriteMany() {
    SpriteGroup = new THREE.Group();
    for (var i = 7; i >= 0; i--) {
        obj = GreatSprite();
        obj.position.set(Math.random() * 2 - 1, Math.random() * 2 - 1, Math.random() * 2 - 1);
        SpriteGroup.add(obj);
    }
    scene.add(SpriteGroup);
}

//粒子运动 Ning+
var TweenSprite;
function TweenSprite(obj) {
    TweenSpriteUP = new TWEEN.Tween(obj.position)
        .to({
            x: obj.position.x,
            y: 2,
            z: obj.position.z
        }, 6000)
        .easing(TWEEN.Easing.Cubic.Out);
    TweenSpriteUP.start();
    TweenSpriteUP.onComplete(function() {
        scene.remove(obj);
    });

    for (var i = obj.children.length - 1; i >= 0; i--) {
        let objMaterial = obj.children[i].material;
        TweenSpriteOpacity1 = new TWEEN.Tween(objMaterial)
            .to({
                opacity: 0.8
            }, 1000)
            .easing(TWEEN.Easing.Cubic.Out);

        TweenSpriteOpacity1.start();
        TweenSpriteOpacity1.onComplete(function() {
            TweenSpriteOpacity2 = new TWEEN.Tween(objMaterial)
                .to({
                    opacity: 0
                }, 1000)
                .easing(TWEEN.Easing.Cubic.Out);
            TweenSpriteOpacity2.start();
        });
    }

}

//粒子发射 Ning+
function CreateEmitter() {
    setInterval("GreatSpriteNew()", "500");
}
{% endcodeblock %}