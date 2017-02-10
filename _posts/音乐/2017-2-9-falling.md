---
layout: post
title: "falling slowly"
date: 2017-2-9
category: 音乐
description: "上星期和同学一起录的，一次成，超开心"
---

<audio controls="controls">
  <source src="/assets/falling.mp3" width=300 height=45 type="audio/mp3" />
Your browser does not support this audio format.
</audio>



<link rel="stylesheet" href="/assets/css/audio.css">
<script type="text/javascript" src="/assets/js/audio.js"></script>

<link rel="stylesheet" href="/assets/audio/css/style.css" media="screen" type="text/css" />
<script type="text/javascript">
window.onload=function(){

   var canvas=document.getElementById('canvas');
   if(canvas.getContext){
		var ctx=canvas.getContext("2d");
		ctx.beginPath();
		ctx.strokeStyle='darkgreen';
		ctx.lineCap='round';
		ctx.lineWidth=6;
		ctx.arc(160,160,150,0,Math.PI,false);
		ctx.stroke();
   }
					   
}
</script>

</head>

<body>
<div id="container">
	<canvas id="canvas" width="320" height="320">对不起，你的浏览器不支持Canvas标签！</canvas>
	<canvas id="progress" width="320" height="320"></canvas><!-- progress bar -->
	<div id="player">
		<audio id="audio" controls>
			<source src="/assets/falling.mp3" type="audio/mpeg" codecs="mp3"></source>		
		</audio>
		<div class="cover">
			<div class="controls">
				<div class="play_pause" id="play" title="Play" onClick="togglePlay()"><i>&#xe600;</i></div>
				<div class="play_pause" id="replay"  onclick="replayAudio()"><i>&#xe607;</i></div>
				<div class="voice"><i>&#xe608;</i><input id="volume" name="volume" min="0" max="1" step="0.1" type="range" onChange="setVolume()" /></div>
				<div id="times">00:00/00:00</div>
			</div><!-- #controls -->
			<div class="info">
				<p class="song"><a href="#" target="_blank">Falling Slowly</a></p>
				<p class="author"><a href="#" target="_blank">Liu Xin</a></p>
			</div>
		</div><!-- #cover -->
	</div><!-- #player -->

</div><!-- #container -->

<script src="/assets/audio/js/index.js"></script>





![1](http://wx3.sinaimg.cn/mw690/8db2c8cbgy1fcl88phzoyj20qo0zk0v7.jpg)
![2](http://wx3.sinaimg.cn/mw690/8db2c8cbgy1fcl89c5hjfj20pg0sxjw7.jpg)
![3](http://wx2.sinaimg.cn/mw690/8db2c8cbgy1fcl891vtg2j211i11itn8.jpg)
![4](http://wx3.sinaimg.cn/mw690/8db2c8cbgy1fcl88mkt1dj20zk0qojtm.jpg)