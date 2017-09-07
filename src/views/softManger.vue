<template>
	<div class="manger">
		<index-headerbtn></index-headerbtn>
 		<index-left></index-left>
    <div class="manger1">
      <div class="manger-tab">
        <el-table
          :data="tableData"
          stripe
          style="width: 100%">
          <el-table-column
            prop="username"
            label="用户名"
            width="">
          </el-table-column>
          <el-table-column
            prop="phonenum"
            label="用户手机号"
            width="">
          </el-table-column>
          <el-table-column
            prop="email"
            label="用户邮箱">
          </el-table-column>     
        </el-table>
      </div>
      <div class="manger-page">
        <el-pagination
          small
          layout="prev, pager, next"
          :total="50" 
          class="manger-page2">
        </el-pagination>
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
      tableData: [{
          username: '滕华伟',
          phonenum: '17681875268',
          email: '17681875268@163.com',
        }, {
          username: '滕华伟',
          phonenum: '17681875268',
          email: '17681875268@163.com',
        }, {
          username: '滕华伟',
          phonenum: '17681875268',
          email: '17681875268@163.com',
        }, {
          username: '滕华伟',
          phonenum: '17681875268',
          email: '17681875268@163.com',
        }
      ]
    }
  },
  components:{
    indexHeaderbtn,
    indexLeft
  }
}
</script>
<style>
  .manger1{
    margin: 20px 20px 0 260px;
    background: #fff;
    height: 500px;
    border-radius: 5px;
  }
  .manger-tab{
    margin: 0 20px;
    padding-top: 40px;
  }
  .manger-page{
    background: #090;
    margin-top: 50px;
  }
  .manger-page2{
    position: absolute;
    left: 50%;
  }
</style>