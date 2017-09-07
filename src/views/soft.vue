<template>
	<div class="hard">
		<index-header></index-header>
 		<index-left></index-left>
    <div class="container">
      <div>
        <router-link class="softaddrouter" to='/softadd'>
          <el-button class="hard-add" type="primary" icon="plus">添加项目信息</el-button>
        </router-link>
      </div>
      <div class="hard-tab">
        <el-table
          :data="tableData"
          stripe
          style="width: 100%">
          <el-table-column
            prop="num"
            label="项目编号">
          </el-table-column>
          <el-table-column
            prop="name"
            label="项目名称"
            width="150">
          </el-table-column>
          <el-table-column
            prop="infor"
            label="中文描述">
          </el-table-column>
          <el-table-column
            prop="componey"
            label="所属公司">
          </el-table-column>
          <el-table-column
            prop="vbanben"
            label="版本信息">
          </el-table-column>
          <el-table-column
            prop="prostatus"
            label="项目状态">
          </el-table-column>
          <el-table-column
            prop="starttime"
            label="创建时间"
            width="110">
          </el-table-column>
          <el-table-column
            prop="endtime"
            label="更新时间"
            width="110">
          </el-table-column>
          <el-table-column
            prop="jiedian"
            label="节点监控"
            width="100">
            <template scope="scope">
              <el-button @click="softjiedian" type="text">查看</el-button>
            </template>
          </el-table-column>
          <el-table-column
            prop="error"
            label="异常通知"
            width="100"
            >
            <template scope="scope">
              <el-button
                 @click="dialogFormVisible = true"
                type="text">
                提醒
              </el-button>
            </template>
          </el-table-column>
          <el-table-column
            prop="controler"
            label="管理者"
            width="100">
            <template scope="scope">
              <el-button @click="softmanger" type="text">查看</el-button>
            </template>
          </el-table-column>
          <el-table-column
            prop="app"
            label="应用监控"
            width="100">
            <template scope="scope">
              <el-button @click="softyyjk" type="text">查看</el-button>
            </template>
          </el-table-column>
          <el-table-column
            prop="status"
            label="状态">
          </el-table-column>
        </el-table>
      </div>
      <div class="hard-page">
        <span class="hard-page1">共123条信息</span>
        <el-pagination
          small
          layout="prev, pager, next"
          :total="50" 
          class="hard-page2">
        </el-pagination>
      </div>
      <!-- 弹出框 -->
      <div>
        <el-dialog title="提醒" :visible.sync="dialogFormVisible"  class="softalert">
          <el-form ref="form" :model="form" label-width="100px" class="softalert1">
            <el-form-item>
              <el-select class="softselect" v-model="form.region" placeholder="数据服务" >
                <el-option label="区域一" value="shanghai"></el-option>
                <el-option label="区域二" value="beijing"></el-option>
              </el-select>
            </el-form-item>
            <el-checkbox-group v-model="form.type">
              <el-checkbox label="邮件提醒" name="type"></el-checkbox>
              <el-checkbox label="短信提醒" name="type"></el-checkbox>
            </el-checkbox-group>
            </el-form-item>
          </el-form>
            <div slot="footer" class="dialog-footer">
              <el-button @click="dialogFormVisible = false">取 消</el-button>
              <el-button type="primary" @click="dialogFormVisible = false">确 定</el-button>
            </div>
          </el-dialog>
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
          num: 'DjuiS5789',
          name: '国网服务器组100',
          infor: '不在服务区',
          componey: '杭州复杂美科技有限公司',
          vbanben: '内测版',
          prostatus: '上线',
          starttime: '2017/12/12 18:00:00',
          endtime: '2017/12/12 18:00:00',
          jiedian: '查看',
          error: '提醒',
          controler: '查看',
          app: '查看',
          status: '运行中'

        }, {
          num: 'DjuiS5789',
          name: '国网服务器组1',
          infor: '不在服务区',
          componey: '杭州复杂美科技有限公司',
          vbanben: '公测版',
          prostatus: '已下线',
          starttime: '2017/12/12 18:00:00',
          endtime: '2017/12/12 18:00:00',
          jiedian: '查看',
          error: '已提醒',
          controler: '查看',
          app: '查看',
          status: '已关闭'
        }, {
          num: 'DjuiS5789',
          name: '国网服务器组1',
          infor: '不在服务区',
          componey: '杭州复杂美科技有限公司',
          vbanben: '正式版',
          prostatus: '已下线',
          starttime: '2017/12/12 18:00:00',
          endtime: '2017/12/12 18:00:00',
          jiedian: '查看',
          error: '已提醒',
          controler: '查看',
          app: '查看',
          status: '已关闭'
        }, {
          num: 'DjuiS5789',
          name: '国网服务器组1',
          infor: '不在服务区',
          componey: '杭州复杂美科技有限公司',
          vbanben: '公测版',
          prostatus: '已下线',
          starttime: '2017/12/12 18:00:00',
          endtime: '2017/12/12 18:00:00',
          jiedian: '查看',
          error: '已提醒',
          controler: '查看',
          app: '查看',
          status: '已关闭'
        }
      ],
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
    }
  },
  components:{
    indexHeader,
    indexLeft
  },
  methods: {
      softjiedian() {
        this.$router.push({path:'/softpoint'})
      },
      softmanger() {
        this.$router.push({path:'/softmanger'})
      },
      softyyjk() {
        this.$router.push({path:'/softyyjk'})
      }
    },
}
</script>
<style>
  .container{
    margin: 20px 20px 0 260px;
    background: #fff;
    height: 500px;
    border-radius: 5px;
  }
  .hard-add{
    float: right;
    width: 130px;
    height: 36px;
    margin: 30px 20px 30px 0 !important;
  }
  .hard-tab{
    margin: 20px 20px 0 20px
  }
  .hard-page{
    background: #090;
    margin-top: 50px;
  }
  .hard-page1{
    float: left;
    margin-left: 40px;
  }
  .hard-page2{
    position: absolute;
    left: 50%;
  }
  .softselect{
    margin-left: -100px;
    width: 350px;
  }
  .softalert{
    width: 820px;
    height: 580px;
    overflow: hidden !important;
    margin: 200px 0 0 550px !important;
  }
  .softalert1{
    width: 450px;
  }
  .softaddrouter{
    text-decoration: none;
    color: #fff;
  }
</style>