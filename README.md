# mobile-move-animate
## 移动端页面整屏滚动动画
### 效果 ：
![image](https://github.com/ZhengYaWei1992/ZWProgressView/blob/master/Untitled3.gif)
https://github.com/issochen/mobile-move-animate/blob/master/1.2019-01-07%2023_28_14.gif
### 下载 直接 引入  <script src="move.js"></script>  即可使用 
### Html 结构
```
 <article class="wrapper">
   <section class="section-1 section">1</section>
   <section class="section-2 section">2</section>
   <section class="section-3 section">3</section>
   <section class="section-4 section">4</section>
   <section class="section-5 section">5</section>
  </article>
```
### css 样式 
```
html, body {
      height: 100%;
      overflow: hidden;
    }
    .wrapper{
      position: absolute;
      width: 100%;
      height: 100%;
    }
    .section{
      width: 100%;
      height: 100%;
    }
    .section-1{
      background: blue;
    }
    .section-2{
      background: yellow;
    }
    .section-3{
      background: red;
    }
    .section-4{
      background: skyblue;
    }
    .section-5{
      background: red;
    }
```
