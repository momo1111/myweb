<template>
  <div class="hello">
  	<img src="../assets/image/person.png" class="image">
  	<div class="topline"></div>
  	<div class="downline"></div>
  	<ul class="nav">
  		<li>
  			<div class="icon icon1"></div>
  			<div class="point point1"></div>
  		</li>
  		<li>
  			<div class="icon icon2"></div>
  			<div class="point point2"></div>
  		</li>
  		<li>
  			<div class="icon icon3"></div>
  			<div class="point point3"></div>
  		</li>
  		<li>
  			<div class="icon icon4"></div>
  			<div class="point point4"></div>
  		</li>
  	</ul>
  	<footer class="footer">
  		<a href="http://www.beian.gov.cn/portal/registerSystemInfo?recordcode=19041418">
  			京ICP备19041418号
  		</a>
  	</footer>
  </div>
</template>
<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style>
	.hello{
		width:100%;
		height:100%;
		position: fixed;
		background:linear-gradient(135deg,rgba(46,48,58,1) 0%,rgba(25,27,33,1) 100%);

	}
	.image{
		position:absolute;
		top:50%;
		left:50%;
		width:500px;
		height:500px;
		transform:translate(-50%,-50%);
		-ms-transform:translate(-50%,-50%); 
		-webkit-transform:translate(-50%,-50%);
	}
	.nav{
		position:fixed;
		top:50%;
		right:60px;
		transform:translate(0%,-50%);
		-ms-transform:translate(0%,-50%); 
		-webkit-transform:translate(0%,-50%);
	}
	.topline{
		width:1px;
		height:18%;
		background:#D8D8D8;
		position:fixed;
		top:0;
		right:91px;
	}
	.downline{
		width:1px;
		height:18%;
		background:#D8D8D8;
		position:fixed;
		bottom:0;
		right:91px;
	}
	.nav li{
		width:64px;
		height:64px;
		list-style:none;
		margin:20px 0;
		position:relative;
	}
	.nav li .icon{
		width:64px;
		height:64px;
		cursor: pointer;
	}
	.point{
		width:95px;
		height:36px;
		position:absolute;
		left:-112px;
		top:14px;
		display:none;
	}
	.nav li:hover .point{
		display:block;
	}
	.nav li .icon1{
		background:url('../assets/image/icon1.png');
		background-size:cover;
		
	}
	.nav li:hover .icon1{
		background:url('../assets/image/hicon1.png');
		background-size:cover;
		
	}
	.nav li .icon2{
		background:url('../assets/image/icon2.png');
		background-size:cover;
	}
	.nav li:hover .icon2{
		background:url('../assets/image/hicon2.png');
		background-size:cover;
		
	}
	.nav li .icon3{
		background:url('../assets/image/icon3.png');
		background-size:cover;
	}
	.nav li:hover .icon3{
		background:url('../assets/image/hicon3.png');
		background-size:cover;
		
	}
	.nav li .icon4{
		background:url('../assets/image/icon4.png');
		background-size:cover;
	}
	.nav li:hover .icon4{
		background:url('../assets/image/hicon4.png');
		background-size:cover;
		
	}
	.nav li .point1{
		background:url('../assets/image/text1.png');
		background-size:cover;
	}
	.nav li .point2{
		background:url('../assets/image/text2.png');
		background-size:cover;
	}
	.nav li .point3{
		background:url('../assets/image/text3.png');
		background-size:cover;
	}
	.nav li .point4{
		background:url('../assets/image/text4.png');
		background-size:cover;
	}
	.footer{
		text-align:center;
		color:#fff;
		width:100%;
		position:absolute;
		bottom:0;
		height:45px;
	    line-height:45px;
		background:#2c2f39;
	}
	.footer a{
		color:#fff;
		text-decoration: none;
		font-size:12px;
	}
</style>
