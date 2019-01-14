# 日誌

在20190107的會議後，為了跨平台的需求以及提高使用者操作、安裝的方便性，決議將遊戲平台轉為瀏覽器，並以javaScript模組作為主要的3D渲染引擎。

目前主流的JS 3D模組有以下幾個：

* p5.js
  * [官網](https://p5js.org/)
* * 操作最簡單，但對3D模組的支援度不如其他的高。
* Three.js
  * [官網](https://threejs.org/)
* * 功能完整、具備製作3D網頁遊戲的API。
  * 支援多種3D繪圖軟體製作的格式。
* BabylonJS
  * [官網](https://www.babylonjs.com/)
* * 微軟釋出的開源3D繪圖框架。

  * 支援Blender、Unity、3DS Max和Maya等3D繪圖軟體製作的格式。

  * [線上編輯器。](http://editor.babylonjs.com/)
* Blend4Web
  * [官網](https://www.blend4web.com/en/)
* * 2018的冬季奧運以Blend4Web，在官網上呈現3D的比賽地圖。

經過多方測驗後，決定以Three.js作為主要得3D模組。  
同時也會嘗試使用BabylonJS，並比較兩者使用上的短版與長處。

---

# Three.js

Three.js將webGL函式進行封裝成一個一個的物件，降低了開發者使用上的難度。

但當需要更細節的操作時，或許仍需要研究webGL的API。

three.js 中基本的繪製流程：

1. 建立場景 \(通常透過 new THREE.Scene\(\)\)
2. 建立物件（mesh\)
   1. 建立幾何形狀
   2. 匯入3D模型
3. 建立材質
4. 加入攝影機
   1. 正交投影與透視投影外，還有 StereoCamera（Perspective Camera ） 以及 CubeCamera （360 度的攝影機）
5. 加入燈光
6. 呼叫 renderer.render 繪製場景。



