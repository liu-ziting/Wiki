# Css相关代码片段集合


#### 自定义滚动条样式

```
::-webkit-scrollbar {
    width: 6px;
    height: 1px;
}

::-webkit-scrollbar-thumb {
  border-radius: 3px;
  -webkit-box-shadow: none;
  background: #f1f1f1;
  -webkit-box-shadow: none;
}

::-webkit-scrollbar-track {
  -webkit-box-shadow: none;
  border-radius: 3px;
  /*background: #06b0b9;*/
  -webkit-box-shadow: none;
}
```

#### 超过部分...

```
-webkit-line-clamp: 2;
display: -webkit-box;
-webkit-box-orient: vertical;
overflow: hidden;
```
#### 隐藏滚动条

```
html {
    overflow: -moz-hidden-unscrollable;
    height: 100%;
}

body::-webkit-scrollbar {
    display: none;
}

body {
    -ms-overflow-style: none;
    height: 100%;
    width: calc(100vw + 18px);
    overflow: auto;
}
```
#### 背景星星特效
##### CSS
```
body {
    background: #22313f;
}
#starsBox {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: rgba(0, 0, 0, 0.75);
    opacity: .5;
}

#starsBox span {
    display: inline-block;
    width: auto;
    position: absolute;
    border-radius: 100%;
    transition: 100s linear;
}
```
##### HTML

```
<div id="starsBox"></div>
```
##### Js

```
var cols = ['#f5d76e', '#f7ca18', '#f4d03f', '#ececec', '#ecf0f1', '#a2ded0'];
var stars = 250;
for(var i = 0; i <= stars; i++) {
    var size = Math.random() * 3;
    var color = cols[parseInt(Math.random() * 4)];
    $('#starsBox').prepend('<span style=" width: ' + size + 'px; height: ' + size + 'px; top: ' + Math.random() * 100 + '%; left: ' + Math.random() * 100 + '%; background: ' + color + '; box-shadow: 0 0 ' + Math.random() * 10 + 'px' + color + ';"></span>');
};
setTimeout(function() {
    $('#starsBox span').each(function() {
        $(this).css('top', Math.random() * 100 + '%').css('left', Math.random() * 100 + '%');
    });
}, 1);
setInterval(function() {
    $('#starsBox span').each(function() {
        $(this).css('top', Math.random() * 100 + '%').css('left', Math.random() * 100 + '%');
    });
}, 100000);
```