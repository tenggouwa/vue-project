<template>
  <div class="soft">
    <index-header></index-header>
    <index-left></index-left>
    <div class="search">
      <el-input class="search-in" v-model="input" placeholder="服务器IP/名称"></el-input>
      <el-button class="search-btn" type="primary" icon="search">搜索</el-button>
      <router-link class="softaddrouter" to='/hardadd'>
        <el-button class="search-add" type="primary" icon="plus">添加服务器</el-button>
      </router-link>
    </div>
    <div class="fuwuqi">
      <div class="fwq-tit">
        <span class="fwq-tit1">国网服务器组1</span>
        <span class="fwq-tit2">2017/12/12 18:00:00</span><span class="fwq-tit2-2">更新时间 : </span>
        <span class="fwq-tit2">2017/12/12 18:00:00</span><span class="fwq-tit2-2">创建时间 : </span>
        <hr class="hr" />
      </div>
      <div class="fwq-container">
        <table>
          <tr>
            <td class="fwq-td1">
              <span class="sp1">机器编号：</span>
              <span class="sp2">dh8874664</span>
            </td>
            <td class="fwq-td1">
              <span class="sp1">外网IP：</span>
              <span class="sp2">192.168.1.1</span>
            </td>
            <td class="fwq-td1">
              <span class="sp1">内网IP：</span>
              <span class="sp2">192.168.1.1</span>
            </td>
            <td class="fwq-td1">
              <span class="sp1">所属公司：</span>
              <span class="sp2">杭州复杂美科技有限公司</span>
            </td>
          </tr>
          <tr>
            <td class="fwq-td1">
              <span class="sp1">CPU信息：</span>
              <span class="sp2">晓龙834</span>
            </td>
            <td class="fwq-td1">
              <span class="sp1">内存容量：</span>
              <span class="sp2">1024MB</span>
            </td>
            <td class="fwq-td1">
              <span class="sp1">硬盘容量：</span>
              <span class="sp2">100TB</span>
            </td>
            <td class="fwq-td2">
              <span class="sp1">服务器用途：</span>
              <span class="sp2">数据服务</span>
            </td>
          </tr>

        </table>
        <div class="fwq-inform">
          <p class="sp1-1">中文描述：</p>
          <p class="sp2-1">这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6</p>
        </div>
      </div>
      <div class="fwq-rongl">
        <div class="jindu1">
          <p>CPU信息</p>
          <el-progress class="jindu2" type="circle" stroke-width="10" :percentage="25"></el-progress>
        </div>
        <div class="jindu1">
          <p>机器内存容量</p>
          <el-progress class="jindu2" type="circle" stroke-width="10" :percentage="35"></el-progress>
        </div>
        <div class="jindu1">
          <p>硬盘容量</p>
        <el-progress class="jindu2" type="circle" stroke-width="10" :percentage="65"></el-progress>
        </div>
      </div>
    </div>
    <div class="fuwuqi">
      <div class="fwq-tit">
        <span class="fwq-tit1">国网服务器组1</span>
        <span class="fwq-tit2">2017/12/12 18:00:00</span><span class="fwq-tit2-2">更新时间 : </span>
        <span class="fwq-tit2">2017/12/12 18:00:00</span><span class="fwq-tit2-2">创建时间 : </span>
        <hr class="hr" />
      </div>
      <div class="fwq-container">
        <table>
          <tr>
            <td class="fwq-td1">
              <span class="sp1">机器编号：</span>
              <span class="sp2">dh8874664</span>
            </td>
            <td class="fwq-td1">
              <span class="sp1">外网IP：</span>
              <span class="sp2">192.168.1.1</span>
            </td>
            <td class="fwq-td1">
              <span class="sp1">内网IP：</span>
              <span class="sp2">192.168.1.1</span>
            </td>
            <td class="fwq-td1">
              <span class="sp1">所属公司：</span>
              <span class="sp2">杭州复杂美科技有限公司</span>
            </td>
          </tr>
          <tr>
            <td class="fwq-td1">
              <span class="sp1">CPU信息：</span>
              <span class="sp2">晓龙834</span>
            </td>
            <td class="fwq-td1">
              <span class="sp1">内存容量：</span>
              <span class="sp2">1024MB</span>
            </td>
            <td class="fwq-td1">
              <span class="sp1">硬盘容量：</span>
              <span class="sp2">100TB</span>
            </td>
            <td class="fwq-td2">
              <span class="sp1">服务器用途：</span>
              <span class="sp2">数据服务</span>
            </td>
          </tr>

        </table>
        <div class="fwq-inform">
          <p class="sp1-1">中文描述：</p>
          <p class="sp2-1">这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6这个服务器很6</p>
        </div>
      </div>
      <div class="fwq-rongl">
        <div class="jindu1">
          <p>CPU信息</p>
          <el-progress class="jindu2" type="circle" stroke-width="10" :percentage="25"></el-progress>
        </div>
        <div class="jindu1">
          <p>机器内存容量</p>
          <el-progress class="jindu2" type="circle" stroke-width="10" :percentage="35"></el-progress>
        </div>
        <div class="jindu1">
          <p>硬盘容量</p>
        <el-progress class="jindu2" type="circle" stroke-width="10" :percentage="65"></el-progress>
        </div>
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
      input:''
    }
  },
  components:{
    indexHeader,
    indexLeft
  }
}
</script>
<style>
body{
  background: #edeff5;
}
  .search{
    margin:20px 20px 0 260px;
    background: #fff;
    border-radius: 5px;
    height: 100px;
  }
  .search-in{
    float: left;
    width: 180px !important;
    height: 36px;
    margin: 30px 10px 0 20px;
  }
  .search-btn{
    float: left;
    width: 79px;
    height: 36px;
    margin-top: 30px !important;
  }
  .search-add{
    float: right;
    width: 130px;
    height: 36px;
    margin: 30px 20px 0 0 !important;
  }
  .fuwuqi{
    margin:20px 20px 0 260px;
    background: #fff;
    border-radius: 5px;
    height: 350px;
  }
  .fwq-tit{
    height: 60px;
    line-height: 60px;
    margin: 0 20px;
  }
  .fwq-tit1{
    font-size: 16px;
    color: #1f2f3d;
    font-weight: bold;
  }
  .fwq-tit2{
    float: right;
    color: #1f2f3d;
  }
  .fwq-tit2-2{
    float: right;
    font-size: 14px;
    color: #bfcbd9;
    margin-left: 30px;
  }
  .fwq-container{
    float: left;
    margin: 42px 0 0 20px;
    width: 900px;
  }
  .fwq-td1{
    width: 230px;
    height: 50px;
  }
  .fwq-td2{
    width: 300px;
    height: 50px;
  }
  .sp1{
    font-size: 14px;
    color: #bfcbd9;
  }
  .sp2{
    font-size: 14px;
    color: #1f2f3d;
  }
  .fwq-inform{
    width: 860px;
    margin-top: 20px;
    /*background: #ccc;*/
  }
  .sp1-1{
    float: left;
    font-size: 14px;
    color: #bfcbd9;
  }
  .sp2-1{
    float: left;
    margin-top: -20px;
    margin-left: 76px;
    font-size: 14px;
    color: #1f2f3d;
  }
  .fwq-rongl{
    float: left;
    margin: 57px 0 0 50px;
  }
  .jindu1{
    float: left;
    margin-left: 40px;
    text-align: center;
  }
  .jindu2{
    margin-top: 30px;
  }
  .hr{
    border: 1px solid #bfcbd9;
  }
</style>