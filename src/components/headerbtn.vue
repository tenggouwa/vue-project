<template>
	<div class="header">
		<h1>后台监控系统</h1>
		<el-button class="gobackbtn" type="info" @click="goback">返回</el-button>
	</div>
	
</template>
<script>
	export default{
		methods:{
			goback(){
				window.history.go(-1);
			}
		}
	}
</script>
<style>
*{
	margin:0;
	padding: 0;
	.header{
	 	width: 100%;
	 	background: #20a0ff;
	 	height: 80px;
	 }
	h1{
		color: #fff;
		font-size: 28px;
		margin-left: 40px;
		line-height: 80px;
	 }
	 .gobackbtn{
	 	border: 1px solid #fff !important;
	 	position: absolute;
	 	right: 50px;
	 	top: 23px;
	 	width: 100px;
	 }
}
</style>