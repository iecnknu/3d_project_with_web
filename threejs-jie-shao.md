# 日誌

在20190107的會議後，為了跨平台的需求以及提高使用者操作、安裝的方便性，決議將遊戲平台轉為瀏覽器，並以javaScript模組作為主要的3D渲染引擎。

目前主流的JS 3D模組有以下幾個：

* p5.js
  * [官網](https://p5js.org/)
* * 操作最簡單，但對3D模組的支援度不如其他的高。
* Three.js
  * [官網](https://threejs.org/)
* * 功能完整、具備製作3D網頁遊戲的API。
* BabylonJS
  * [官網](https://www.babylonjs.com/)
* * 微軟釋出的開源3D繪圖框架。
* Blend4Web
  * [官網](https://www.blend4web.com/en/)
* * 2018的冬季奧運以Blend4Web，在官網上呈現3D的比賽地圖。

經過多方測驗後，決定以Three.js作為主要得3D模組。  
同時也會嘗試使用BabylonJS。

# Three.js

Three.js將webGL函式進行封裝成一個一個的物件，降低了開發者使用上的難度。

但當需要更細節的操作時，或許仍需要研究webGL的API。



