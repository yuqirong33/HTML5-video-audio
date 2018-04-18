# HTML5-video-audio

问题：     
调用摄像头问题：     
1.使用原生  javascript:     
 navigator.mediaDevices.getUserMedia  方法调用手机前置摄像头     
在调试的过程中电脑端谷歌浏览器手机控制台可以获取到摄像头     
在安卓真机上可以获取到前置摄像头     
在iOS真机上不支持摄像头的调用 （官方说的是iOS版本11以上是可以的，但是实际是不行）     
演示地址：https://119.90.43.106:9792/vpr/HTML-yqr/index.html     

2.使用 input     
<input type="file" name="file" accept="image/*" capture="camera"> 获取摄像头     
都能获取到摄像头  安卓和iOS体验效果太差     
演示地址：https://119.90.43.106:9792/vpr/HTML-yqr/index3.html     

3.使用第三方库 tracking.js     
在安卓真机上可以获取到前置摄像头     
在调试的过程中电脑端谷歌浏览器手机控制台可以获取到摄像头     
在iOS真机上不支持摄像头的调用（官方说的是iOS版本11以上是可以的，但是实际是不行）     
演示地址：https://119.90.43.106:9792/vpr/HTML-yqr/index2.html     


调用音频问题：     
1.使用  HTML5  提供的  audio  标签不能支持iOS     
 	演示地址：https://119.90.43.106:9792/vpr/HTML-yqr/video2.html     

2.使用原生  javascript:     
        navigator.mediaDevices.getUserMedia  方法获取音频流     
在调试的过程中电脑端谷歌浏览器手机控制台可以获取到音频流     
在安卓与iOS真机上不支持音频流的调用      
演示地址：https://119.90.43.106:9792/vpr/HTML-yqr/video.html     

3.使用 Audio5js - HTML5音频兼容层 尝试解决移动端兼容性问题     
       使用 audio5js.swf 播放器的音频编解码器     
       在电脑端是可以支持音频效果的     
       在安卓和iOS真机下不支持     
       演示地址：https://119.90.43.106:9792/vpr/HTML-yqr/video3.html     
  

其他解决方案（暂未尝试）：     
1.使用微信  JS-SDK  接口调用音频接口可以实现音频视频     
演示地址：http://203.195.235.76/jssdk/   （必须在微信中才能使用）     

2.使用 iH5  在线制作H5工具可以实现音频  （不推荐，受局限）     

3.使用 HTML5 开发工具 hbuilder 调用硬件的功能，实现原生的效果     
