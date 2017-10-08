# css
一些css的读书笔记
![image](https://github.com/pathoner/css/blob/master/images/1.png)
怎么实现上述照片的布局呢？
``` html
<!DOCTYPE html>
<html>
<head>
  <title>定位和居中</title>
  <meta charset="utf-8">
  <style type="text/css">
    .content {
      width: 400px;
      height: 200px;
      border: 1px solid black;
      position: absolute;
      top:50%;
      left: 50%;
      transform: translate(-50%, -50%);
    }
    .quarter-circle {
      width: 50px;
      height: 50px;
      background-color: #FC0;
      position: absolute;
    }
    .l {
      top: 0;
      left: 0;
      border-bottom-right-radius: 100%;
    }
    .r {
      bottom: 0;
      right: 0;
      border-top-left-radius: 100%;
    }
  </style>
}
</head>
<body>
  <div class="content">
    <div class="quarter-circle l"></div>
    <div class="quarter-circle r"></div>
  </div>
</body>
</html>
```
