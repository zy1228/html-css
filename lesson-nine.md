# Adding Media

## 添加图像
    <img src="dog.jpg" alt="A black, brown, and white dog wearing a kerchief">
    
图像的格式：
（1）GIF：动图
（2）jpg：高色彩的高质量图像，同时保持适当的文件大小，非常适合更快的加载时间，如照片
（3）png：具有透明度或低颜色计数的图像，如背景图片或图标
alt一般用于描述图像的属性，用于图像丢失时便于寻找图像

## 调整图像大小
    img {
      height: 200px;
      width: 200px;
    }

## 定位图像
默认情况下，图像被定位为内联级元素，但位置可以被CSS改变。

这是一段默认情况下图片显示位置的代码    

    <p>Gatsby is a black, brown, and white hound mix puppy who loves howling at fire trucks and collecting belly rubs. <img src="dog.jpg" alt="A black, brown, and white dog wearing a kerchief"> Although he spends most of his time sleeping he is also quick to chase any birds who enter his vision.</p>

块定位：

    img {
      display: block;
    }

浮动定位：

    img {
      background: #eaeaed;
      border: 1px solid #9799a7;
      float: right;
      margin: 8px 0 0 20px;
      padding: 4px;
    }

## 添加音频    
音频属性：autoplay，controls，loop，和preload。
默认情况下，不会显示。
autoplay：会在加载时自动播放。
controls：显示元素
loop：导致音频文件从头到尾不断重复。
preload：属性有助于识别在播放剪辑之前应加载有关音频文件的信息，有三个值，none 不显示、auto 预加载所有信息、metadata预加载有关音频文件的任何可用元数据信息，例如剪辑的长度


## 添加视频

添加视频与音频相似，只是将audio属性置换成video属性

此外还有一个海报属性poster，用于视频播放前的界面显示。
  
    <video src="earth.ogv" controls poster="earth-video-screenshot.jpg"></video>

## 回退

每个浏览器支持不同的音频格式，为了让各个浏览器兼容，使用音频回退。

    <audio controls>
      <source src="jazz.ogg" type="audio/ogg">
      <source src="jazz.mp3" type="audio/mpeg">
      <source src="jazz.wav" type="audio/wav">
      Please <a href="jazz.mp3" download>download</a> the audio file.
    </audio>

当加载到适合的格式时，将会忽略其他文件。
当浏览器不支持audio元素时，可提供一个链接。

视频回退

    <video controls>
      <source src="earth.ogv" type="video/ogg">
      <source src="earth.mp4" type="video/mp4">
      Please <a href="earth.mp4" download>download</a> the video.
    </video>

## 添加内联框架

将另一个html页面嵌入当前页面中

    <iframe src="https://www.baidu.com"></iframe>

## 语义

figure元素：在语义上标记自包含的内容或媒体
figcaption元素：在figure元素中添加标题或图例




















