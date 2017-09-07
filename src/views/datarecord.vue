<template>
	<div class="datarecord">
		<index-header></index-header>
 		<index-left></index-left>
    <div class="datarecord1">
      <div class="datarecord1-tit">国网服务器组1<hr class="hr-1"></div>
      <div class="datarecord1-con">
        <span class="datarecord1-sp1">每秒交易数:</span>
        <span class="datarecord1-sp2">dh8874664</span>
        <span class="datarecord1-sp1">用户注册量:</span>
        <span class="datarecord1-sp2">XXXXX</span>      
      </div>
    </div>
    <div class="datarecord1">
      <div class="datarecord1-tit">国网服务器组1<hr class="hr-1"></div>
      <div class="datarecord1-con">
        <span class="datarecord1-sp1">每秒交易数:</span>
        <span class="datarecord1-sp2">dh8874664</span>
        <span class="datarecord1-sp1">用户注册量:</span>
        <span class="datarecord1-sp2">XXXXX</span>      
      </div>
    </div>
    <div class="datarecord1">
      <div class="datarecord1-tit">国网服务器组1<hr class="hr-1"></div>
      <div class="datarecord1-con">
        <span class="datarecord1-sp1">每秒交易数:</span>
        <span class="datarecord1-sp2">dh8874664</span>
        <span class="datarecord1-sp1">用户注册量:</span>
        <span class="datarecord1-sp2">XXXXX</span>      
      </div>
    </div>
   
    
 	</div>

</template>
<script>
import indexHeader from '../components/header.vue'
import indexLeft from '../components/left.vue'
export default {
  // name: 'hello',
  data () {
    return {
      input:'',
      }
  },
  components:{
    indexHeader,
    indexLeft
  }
}
</script>
<style>
  .datarecord1{
    margin: 20px 20px 0 260px;
    background: #fff;
    height: 84px;
    line-height: 84px;
    border-radius: 5px;
  }
  .datarecord1{
    height: 120px;
    background: #fff;
    margin: 20px 20px 0 260px;
    border-radius: 5px;
  }
  .datarecord1-tit{
    margin: 0 20px;
    height: 60px;
    line-height: 60px;
    font-size: 16px;
    font-weight: bold;
  }
  .datarecord1-con{
    margin:0 20px;
     height: 60px;
    line-height: 60px;
  }
  .datarecord1-sp1{
    color: #bfcbd9;
    text-align: center;
  }
  .datarecord1-sp2{
    color: #1f2f3d;
    width: 40%;
    display: inline-block;
  }
</style>