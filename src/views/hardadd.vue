<template>
	<div class="hardadd">
		<index-headerbtn></index-headerbtn>
 		<index-left></index-left>
    <div class="hardadd1">
      <p>添加服务器</p>
      <div class="hardadd1for">
        <el-form ref="form" :model="form" label-width="100px" class="hardadd1form">
          <el-form-item label="服务器名称:">
            <el-input v-model="form.name"></el-input>
          </el-form-item>
          <el-form-item label="机器编号:">
            <el-input v-model="form.name"></el-input>
          </el-form-item>
          <el-form-item label="外网IP:">
            <el-input v-model="form.name"></el-input>
          </el-form-item>
          <el-form-item label="内网IP:">
            <el-input v-model="form.name"></el-input>
          </el-form-item>
          <el-form-item label="所属公司:">
            <el-input v-model="form.name"></el-input>
          </el-form-item>
          <el-form-item label="CPU信息:">
            <el-input v-model="form.name"></el-input>
          </el-form-item>
          <el-form-item label="内存容量:">
            <el-input v-model="form.name"></el-input>
          </el-form-item>
          <el-form-item label="硬盘容量:">
            <el-input v-model="form.name"></el-input>
          </el-form-item>
          <el-form-item label="服务器用途:">
            <el-select class="addselect1" v-model="form.region" placeholder="数据服务">
              <el-option label="区域一" value="shanghai"></el-option>
              <el-option label="区域二" value="beijing"></el-option>
            </el-select>
          </el-form-item>
          <el-form-item label="数据端口:">
            <el-input v-model="form.name"></el-input>
          </el-form-item>
          <el-form-item label="中文描述:">
            <el-input type="textarea" v-model="form.desc"></el-input>
          </el-form-item>
          <el-form-item>
            <el-button type="primary" @click="onSubmit">确定</el-button>
            <el-button>取消</el-button>
          </el-form-item>
        </el-form>
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
        form: {
          // name: '',
          // region: '',
          // date1: '',
          // date2: '',
          // delivery: false,
          // type: [],
          // resource: '',
          // desc: ''
        }
      }
  },
  components:{
    indexHeaderbtn,
    indexLeft
  }
}
</script>
<style>
  .hardadd1{
    margin: 20px 20px 0 260px;
    background: #fff;
    line-height: 84px;
    border-radius: 5px;
  }
  .hardadd1 p{
    margin: 30px 0 0 32px;
    font-size: 16px;
    color: #1f2f3d;
    font-weight: bold;
  }
  .hardadd1for{
    margin-left: 100px;
  }
  .hardadd1form{
    width: 450px;
    display: inline-block !important;
  }
  .addselect1{
    width: 350px;
  }
</style>