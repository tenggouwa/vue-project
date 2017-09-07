<template>
	<div class="softpoint">
		<index-headerbtn></index-headerbtn>
 		<index-left></index-left>
    <div class="softpoint1">
      <p>节点高度：#387031</p>
    </div>
    <div class="softpoint2">
      <div class="softpoint2-tit">国网服务器组1<hr class="hr-1"></div>
      <div class="softpoint2-con">
        <span class="point-sp1">节点高度:</span>
        <span class="point-sp2">dh8874664</span>
        <span class="point-sp1">访问状态:</span>
        <span class="point-sp2">XXXXX</span>
        <span class="point-sp1">API状态:</span>
        <span class="point-sp2">XXXXX</span>
        <span class="point-sp1">API访问状况:</span>
        <span class="point-sp2">XXXXX</span>
        <span class="point-sp1">是否匹配:</span>
        <span class="point-sp2">是</span>
        <span class="point-sp1">状态:</span>
        <span class="point-sp2">已重启</span>
      </div>
    </div>
    <div class="softpoint2">
      <div class="softpoint2-tit">国网服务器组1<hr class="hr-1"></div>
      <div class="softpoint2-con">
        <span class="point-sp1">节点高度:</span>
        <span class="point-sp2">dh8874664</span>
        <span class="point-sp1">访问状态:</span>
        <span class="point-sp2">XXXXX</span>
        <span class="point-sp1">API状态:</span>
        <span class="point-sp2">XXXXX</span>
        <span class="point-sp1">API访问状况:</span>
        <span class="point-sp2">XXXXX</span>
        <span class="point-sp1">是否匹配:</span>
        <span class="point-sp2">是</span>
        <span class="point-sp1">状态:</span>
        <span class="point-sp2">已重启</span>
      </div>
    </div>
    <div class="softpoint2">
      <div class="softpoint2-tit">国网服务器组1<hr class="hr-1"></div>
      <div class="softpoint2-con">
        <span class="point-sp1">节点高度:</span>
        <span class="point-sp2">dh8874664</span>
        <span class="point-sp1">访问状态:</span>
        <span class="point-sp2">XXXXX</span>
        <span class="point-sp1">API状态:</span>
        <span class="point-sp2">XXXXX</span>
        <span class="point-sp1">API访问状况:</span>
        <span class="point-sp2">XXXXX</span>
        <span class="point-sp1">是否匹配:</span>
        <span class="point-sp2">是</span>
        <span class="point-sp1">状态:</span>
        <span class="point-sp2">已重启</span>
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
  .softpoint1{
    margin: 20px 20px 0 260px;
    background: #fff;
    height: 84px;
    line-height: 84px;
    border-radius: 5px;
  }
  .softpoint1 p{
    margin-left: 20px;
    font-size: 24px;
  }
  .softpoint2{
    height: 120px;
    background: #fff;
    margin: 20px 20px 0 260px;
    border-radius: 5px;
  }
  .softpoint2-tit{
    margin: 0 20px;
    height: 60px;
    line-height: 60px;
    font-size: 16px;
    font-weight: bold;
  }
  .softpoint2-con{
    margin:0 20px;
     height: 60px;
    line-height: 60px;
  }
  .point-sp1{
    color: #bfcbd9;
  }
  .point-sp2{
    color: #1f2f3d;
    width: 180px;
    display: inline-block;
  }
  .hr-1{
    border-top: 1px solid #ccc;
  }
</style>