<template><!--模板：页面内容、元素、组件都写在这里-->
<div class="first"><!--div组件定义一个父容器-->
    <text class="test">hhh</text>
    <text class="message">kkk</text>
	<image class="img" src="/img/a.jpg"></image>

	<div class="second">
		<div class="box1"></div>
		<div class="box2"></div>
	</div>
	<a href="../dist/vendor.web.js">
		<text>jump</text>
	</a>
	<div class="webtest">
		<web class="web" :src="src1"></web>
	</div>
</div>
</template>
<style>
	.message{height: 100px;width: 100px;background-color: red;position: relative;}
	.test{height: 100px;width: 100px;border-width: 10px;border-color: black;border-style: solid;background-image:linear-gradient(to bottom,green,yellow);position: relative;}
	.img{height: 100px;border-radius: 20px;}
	.box1{height: 100px;width:50px;background-color: blue}
	.box2{height: 100px;width: 50px;background-color: pink}
	.second{flex-direction: row;}/*weex默认flex的布局，每个元素有默认的dispaly：flex;不需要重新定义*/
	.webtest{height: 300px;width: 750px;}
	.web{height: 300pa;width: 750px;}
</style>

<script>
export default {
	data:{
		src1:"http://imooc.com"
	}
}
</script>

