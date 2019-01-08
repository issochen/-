# mobile-move-animate
## 移动端页面整屏滚动动画
### 效果 ：(gif 太卡了 没制作好)
![image](https://github.com/issochen/mobile-move-animate/blob/master/1.2019-01-07%2023_28_14.gif)

### 用法
    引入 <script src="move.js"></script>  
    const fullPage = new FullPage(".wrapper") 即可使用 
    如果需要与某个点击按钮关联起来
    只需调用 fullPage.changeNum(num) 方法  num为你需要跳转到哪一屏的 页码
    列如：
    ```
      firstArrow.addEventListener('click', function(){
        const totalY = document.documentElement.clientHeight || document.body.clientHeight
        fullPage.changeNum(2)
        twoScreen.style.transition = 'all .5s'
        twoScreen.style.transform = `translateY(-${totalY}px)`
      })
    ```
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
