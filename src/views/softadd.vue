<template>
	<div class="softadd">
		<index-headerbtn></index-headerbtn>
 		<index-left></index-left>
    <div class="softadd1">
      <div class="softadd1-1">      
        <el-form ref="form" :model="form" label-width="100px" class="softadd1form">
        <!-- 添加项目信息 -->
        <p class="softadd1forp">添加项目信息</p>
          <el-form-item label="项目编号:">
            <el-input v-model="form.name"></el-input>
          </el-form-item>
          <el-form-item label="项目名称:">
            <el-input v-model="form.name"></el-input>
          </el-form-item>
          <el-form-item label="中文描述:">
            <el-input v-model="form.name"></el-input>
          </el-form-item>
          <el-form-item label="所属公司:">
            <el-input v-model="form.name"></el-input>
          </el-form-item>
          <el-form-item label="版本信息:">
            <el-select class="addselect1" v-model="form.region">
              <el-option label="内测版" value="shanghai"></el-option>
              <el-option label="公测版" value="beijing"></el-option>
            </el-select>
          </el-form-item>
          <el-form-item label="项目状态:">
            <el-select class="addselect1" v-model="form.region">
              <el-option label="上线" value="shanghai"></el-option>
              <el-option label="区域二" value="beijing"></el-option>
            </el-select>
          </el-form-item>
          <!-- 添加关联服务器 -->
          <p class="softadd1forp">添加关联服务器</p>
          <el-form-item class="addfwq" label="服务器:">
            <el-select class="addselect1" v-model="form.region">
              <el-option label="服务器1" value="shanghai"></el-option>
              <el-option label="服务器2" value="beijing"></el-option>
            </el-select>
          </el-form-item>
          <el-button class="addfwq1" type="primary" icon="plus"  @click="dialogFormVisible = true">添加服务器</el-button>
          <!-- 添加管理者 -->
          <p class="softadd1forp">添加管理者</p>
          <el-form-item label="姓名:">
            <el-input v-model="form.name"></el-input>
          </el-form-item>
          <el-form-item label="邮箱:">
            <el-input v-model="form.name"></el-input>
          </el-form-item>
          <el-form-item label="手机号:">
            <el-input v-model="form.name"></el-input>
          </el-form-item>
          <el-form-item class="addformbtn">
            <el-button class="addformbtn1" type="primary" @click="onSubmit">确定</el-button>
            <el-button class="addformbtn2">取消</el-button>
          </el-form-item>
        </el-form>
      </div>
    </div>
    
    <!-- 弹出框 -->
    <el-dialog title="添加服务器" :visible.sync="dialogFormVisible"  class="softadd1alert">
      <el-form ref="form" :model="form" label-width="100px" class="softadd1alert1">
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
        </el-form>
      <div slot="footer" class="dialog-footer">
        <el-button @click="dialogFormVisible = false">取 消</el-button>
        <el-button type="primary" @click="dialogFormVisible = false">确 定</el-button>
      </div>
    </el-dialog>

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
        },
        dialogTableVisible: false,
        dialogFormVisible: false,
        form: {
          name: '',
          region: '',
          date1: '',
          date2: '',
          delivery: false,
          type: [],
          resource: '',
          desc: ''
        },
        formLabelWidth: '120px'
      };
      },
      components:{
        indexHeaderbtn,
        indexLeft
  }
  }
  

</script>
<style>
  .softadd1{
    margin: 20px 20px 0 260px;
    background: #fff;
    border-radius: 5px;
  }
  .softadd1-1{
    margin: 30px 0 0 32px;
  }
  .softadd1forp{
    line-height: 80px;
    font-size: 16px;
    color: #1f2f3d;
    font-weight: bold;
    margin-left: -50px;
  }
  .softadd1form{
    margin: 0px 0 0 52px;
    width: 450px;
    display: inline-block !important;
  }
  .addfwq1{
    float: right;
    margin-right: -140px !important;
    margin-top: -58px !important;
  }
  .addformbtn1{
    float: right;
  }
  .addformbtn2{
    float: right;
    margin-right: 20px !important;
  }
  .softadd1alert{
    width: 1100px;
    overflow: hidden !important;
    margin: -100px 0 0 400px !important;
  }
  .softadd1alert1{
    width: 450px;
  }
</style>