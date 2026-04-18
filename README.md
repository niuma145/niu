<!DOCTYPE html>
<html lang="zh-CN">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
<meta name="apple-mobile-web-app-capable" content="yes">
<title>牛马的爱心</title>
<style>
*{margin:0;padding:0;}
html,body{width:100%;height:100%;overflow:hidden;background:#000;}
iframe{width:100%;height:100%;border:none;}
/*加载遮罩，网差/打不开全程黑屏盖住*/
.load-bg{position:fixed;top:0;left:0;width:100%;height:100%;background:#000;z-index:99;}
</style>
</head>
<body>
<div class="load-bg" id="loading"></div>
<iframe id="miframe" sandbox="allow-scripts allow-same-origin allow-forms allow-popups allow-top-navigation"></iframe>

<script>
const iframe = document.getElementById('miframe');
const load = document.getElementById('loading');
//隐蔽写入地址，源码抓不到外链
iframe.src = 'http://a.u9c.cn/6qyDll';

//加载成功才消失遮罩
iframe.onload = function(){
  load.style.display='none';
}
//加载失败/断网，一直黑屏，绝不露出原链接
iframe.onerror = function(){
  load.style.display='block';
}
</script>
</body>
</html>