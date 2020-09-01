d# 学习笔记

## 1.1 准备工作

* Three.js是一个JavaScript库

## 1.2 获取源码

* 教程源码的地址 ` https://github.com/josdirksen/learning-threejs `

## 1.3 搭建HTML框架

* 至少包含Three.js库
* TrackballControl.js，控制器库，可以利用鼠标任意移动摄像机以便从不同角度观察场景
* body标签中包含一个div元素：` <div id =webgl-output"></div> `，Three.js渲染器的输出指向这个元素
* Three.js有两个不同的版本：
  * three.min.js，一般用于网上部署，使用UglifyJS压缩过的，大小是普通Three.js四分之一
  * three.js，普通的Three.js库，为了便于进行代码调试和理解Three.js的源码

## 1.4 渲染并查看三维对象

* 场景（scene），一个容器，主要用于保存、跟踪所要渲染的物体和使用的光源
* 摄像机（camera），决定了能够在场景看到什么
* 渲染器（renderer），基于摄像机的角度来计算场景对象在浏览器中会渲染成什么样子
* WebGLRenderer将会使用电脑显卡来渲染场景
* 除了基于WebGL的渲染器外，还有其他渲染器，比如基于HTML canvas的渲染器、基于CSS的渲染器、甚至还有基于SVG的渲染器。但是不推荐使用，已停止更新而且十分耗CPU资源
* THREE.Scene，创建场景对象
* THREE.PerspectiveCamra，创建摄像机对象
* THREE.WebGLRender，创建渲染器对象
* THREE.AxesHelper，创建坐标轴对象
* THREE.PlaneGeometry，创建平面对象
* THREE.MeshBasicMaterial，创建基本材质

## 1.5 添加材质、光源和阴影效果

* THREE.SpotLight，定义光源
* 基本材质指挥使用指定的颜色来渲染物体
* Three.js中MeshPhysicalMaterial和MeshStandardMaterial在渲染时会对光源产生反应

## 1.6 让你的场景动起来

## 1.7 使用dat.GUI简化试验流程

## 1.8 场景对浏览器的自适应
