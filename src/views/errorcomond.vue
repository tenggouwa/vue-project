<template>
	<div class="errorcomond">
		<index-header></index-header>
 		<index-left></index-left>
    <div class="errorcomond1">
      <div class="error-tab">
        <el-table
          :data="tableData"
          stripe
          style="width: 100%">
          <el-table-column
            prop="num"
            label="记录号"
            width="">
          </el-table-column>
          <el-table-column
            prop="namenum"
            label="项目编号"
            width="">
          </el-table-column>
          <el-table-column
            prop="mnum"
            label="机器编号">
          </el-table-column>
          <el-table-column
            prop="vinfor"
            label="版本信息">
          </el-table-column>
          <el-table-column
            prop="errorinfor"
            label="异常信息">
          </el-table-column>
          <el-table-column
            prop="chulistatus"
            label="处理状态">
          </el-table-column>
          <el-table-column
            prop="starttime"
            label="创建时间">
          </el-table-column>
          <el-table-column
            prop="endtime"
            label="更新时间">
          </el-table-column>
        </el-table>
      </div>
      <div class="hard-page">
        <el-pagination
          small
          layout="prev, pager, next"
          :total="50" 
          class="hard-page2">
        </el-pagination>
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
      tableData: [{
          num: '123456',
          namenum: '123456',
          mnum: '123456',
          vinfor: '硬件异常',
          errorinfor: '待处理',
          chulistatus: '状态正常',
          starttime: '2017/12/12 18:00:00',
          endtime: '2017/12/12 18:00:00',
        }, {
          num: '123456',
          namenum: '123456',
          mnum: '123456',
          vinfor: '软件异常',
          errorinfor: '待处理',
          chulistatus: '状态正常',
          starttime: '2017/12/12 18:00:00',
          endtime: '2017/12/12 18:00:00',
        }, {
          num: '123456',
          namenum: '123456',
          mnum: '123456',
          vinfor: '硬件异常',
          errorinfor: '已处理',
          chulistatus: '状态正常',
          starttime: '2017/12/12 18:00:00',
          endtime: '2017/12/12 18:00:00',
        }, {
          num: '123456',
          namenum: '123456',
          mnum: '123456',
          vinfor: '硬件异常',
          errorinfor: '待处理',
          chulistatus: '状态正常',
          starttime: '2017/12/12 18:00:00',
          endtime: '2017/12/12 18:00:00',
        }
      ]
    }
  },
  components:{
    indexHeader,
    indexLeft
  }
}
</script>
<style>
  .errorcomond1{
    margin: 20px 20px 0 260px;
    background: #fff;
    height: 500px;
    border-radius: 5px;
  }
  .error-tab{
    margin: 0 20px;
    padding-top: 40px;
  }
  .hard-page{
    background: #090;
    margin-top: 50px;
  }
  .hard-page2{
    position: absolute;
    left: 50%;
    /*margin-left: -70px;*/
  }
</style>