<template>
	<div class="left">
		<el-col class="left-1">
		   <!--  <el-menu default-active="2" class="el-menu-vertical-demo" @open="handleOpen" @close="handleClose" theme="dark"> -->
		   <!-- <el-menu :default-active="$route.path" mode="vertical" default-active="2" class="el-menu-vertical-demo" theme="dark" router> -->
		   <el-menu :default-active="$route.path" class="el-menu-vertical-demo" theme="dark" router>
		        <!-- <el-submenu index="1" class="nav">
		          	<template slot="title">硬件监控</template>
			        <el-menu-item index="1-1"><router-link class="leftrouter" to='/hard'>服务器列表</router-link></el-menu-item>
		        </el-submenu>
		        <el-submenu index="2" class="nav">
		          	<template slot="title">软件监控</template>
			        <el-menu-item index="2-1"><router-link class="leftrouter" to='/soft'>项目列表</router-link></el-menu-item>
		        </el-submenu>
		        <el-submenu index="3" class="nav">
		          	<template slot="title">数据统计</template>
			        <el-menu-item index="3-1"><router-link class="leftrouter" to='/datarecord'>数据统计表</router-link></el-menu-item>
		        </el-submenu>
		        <el-submenu index="4" class="nav">
		          	<template slot="title">异常记录</template>
			        <el-menu-item index="4-1"><router-link class="leftrouter" to='/errorcomond'>异常日志</router-link></el-menu-item>
		        </el-submenu>		 -->
		        <el-menu-item index="/hard" class="leftmenu"><i class="el-icon-setting leftico" ></i>硬件监控</el-menu-item>
        		<el-menu-item index="/soft" class="leftmenu"><i class="el-icon-menu leftico"></i>软件监控</el-menu-item>        
        		<el-menu-item index="/datarecord" class="leftmenu"><i class="el-icon-date leftico"></i>数据统计</el-menu-item>
        		<el-menu-item index="/errorcomond" class="leftmenu"><i class="el-icon-information leftico"></i>异常记录</el-menu-item> 
		    </el-menu>
		</el-col>
	</div>
</template>
<script>
	export default {
	    // methods: {
	    //     lefthard() {
		   //     this.$router.push({path:'/hard'})
		   //  },
		   //  leftsoft() {
		   //     this.$router.push({path:'/soft'})
		   //  },
		   //  leftdata() {
		   //     this.$router.push({path:'/datarecord'})
		   //  },
		   //  lefterror() {
		   //     this.$router.push({path:'/errorcomond'})
		   //  }
	    // }
    }
</script>
<style>
	body{
		/*overflow: hidden;*/
	}
	.leftrouter{
		text-decoration: none;
		color: #20A0FF;
		padding: 16px 85px 16px 80px;
		margin-left: -40px;
	}
	.left-1{
		background: #324157;
		width: 240px !important;
		height: 1000px;
		float: left;
	}
	.nav{
		width: 240px;
	}
	.leftmenu{
		height: 60px !important;
		line-height: 60px !important;
		font-size: 16px !important;
	}
	.leftico{
		margin-right: 50px !important;
	}
</style>