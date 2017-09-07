<template>
	<div class="softyyjk">
		<index-headerbtn></index-headerbtn>
 		<index-left></index-left>
    <div class="softyyjk1">
      <div class="softyyjk1-tit">国网服务器组1<hr class="hr-1"></div>
      <div class="softyyjk1-con">
        <span class="yyjk-sp1">节点高度:</span>
        <span class="yyjk-sp2">dh8874664</span>
        <span class="yyjk-sp1">访问状态:</span>
        <span class="yyjk-sp2">XXXXX</span>
        <span class="yyjk-sp1">软件服务器状态:</span>
        <span class="yyjk-sp2">在线</span>        
      </div>
    </div>
    <div class="softyyjk1">
      <div class="softyyjk1-tit">国网服务器组1<hr class="hr-1"></div>
      <div class="softyyjk1-con">
        <span class="yyjk-sp1">节点高度:</span>
        <span class="yyjk-sp2">dh8874664</span>
        <span class="yyjk-sp1">访问状态:</span>
        <span class="yyjk-sp2">XXXXX</span>
        <span class="yyjk-sp1">软件服务器状态:</span>
        <span class="yyjk-sp2">在线</span>        
      </div>
    </div>
    <div class="softyyjk1">
      <div class="softyyjk1-tit">国网服务器组1<hr class="hr-1" ></div>
      <div class="softyyjk1-con">
        <span class="yyjk-sp1">节点高度:</span>
        <span class="yyjk-sp2">dh8874664</span>
        <span class="yyjk-sp1">访问状态:</span>
        <span class="yyjk-sp2">XXXXX</span>
        <span class="yyjk-sp1">软件服务器状态:</span>
        <span class="yyjk-sp2">在线</span>        
      </div>
    </div>
 	</div>

</template>
<script>
import indexHeaderbtn from '../components/headerbtn.vue'
import indexLeft from '../components/left.vue'
export default {
  // name: 'hello',
  data () {
    return {
      input:'',
      }
  },
  components:{
    indexHeaderbtn,
    indexLeft
  }
}
</script>
<style>
  .softyyjk1{
    margin: 20px 20px 0 260px;
    background: #fff;
    height: 84px;
    line-height: 84px;
    border-radius: 5px;
  }
  .softyyjk1{
    height: 120px;
    background: #fff;
    margin: 20px 20px 0 260px;
    border-radius: 5px;
  }
  .softyyjk1-tit{
    margin: 0 20px;
    height: 60px;
    line-height: 60px;
    font-size: 16px;
    font-weight: bold;
  }
  .softyyjk1-con{
    margin:0 20px;
     height: 60px;
    line-height: 60px;
  }
  .yyjk-sp1{
    color: #bfcbd9;
    text-align: center;
  }
  .yyjk-sp2{
    color: #1f2f3d;
    width: 27%;
    display: inline-block;
  }
</style>