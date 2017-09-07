<template>
  <div class="hello">
    <div class="login">
      <p>监控后台管理系统</p>
      <div class="username">
        <img class="user" src="../assets/img/User.png" height="24" width="23">
        <span class="user1">用户名</span>
        <input class="user2" type="text">
      </div>
      <div class="password">
        <img class="key" src="../assets/img/Key.png" height="24" width="25">
        <span class="key1">密码</span>
        <input class="key2" type="text">
      </div>
     <div class="remember">
        <el-checkbox label="记住用户名和密码" name="type"></el-checkbox>
     </div>
     <div class="loginbtn">
       <el-button class="loginbtn1" type="primary" @click="loginbtn">登 录</el-button>
     </div>
    </div>
  </div>
</template>

<script>
import indexHeader from '../components/header.vue'
import indexLeft from '../components/left.vue'
export default {
  name: 'hello',
  data () {
    return {
      msg: 'index'
    }
  },
  methods:{
    loginbtn() {
      alert("你想登陆吗？叫一声爸爸再点击确定就好了！");
        this.$router.push({path:'/hard'})
      }
  }
}
</script>
<style>
body{
  /*overflow:hidden;*/
  height: 100%;
}
.hello{
  width: 100%;
  height: 100vh;
  background: url(../assets/img/background.jpg) no-repeat;
  background-size: 100% 100%; 
}
.login{
  width: 537px;
  height: 458px;
  background: #fff;
  position: absolute;
  top: 50%;
  left: 50%;
  margin: -229px 0 0 -268px;
  box-shadow:  0px 0px 30px 30px rgba(80,138,248,0.3);
}
.login p{
  font-size: 24px;
  color: #20A0FF;
  text-align: center;
  margin-top: 46px;
}
.username{
  height: 50px;
  width: 450px;
  line-height: 50px;
  margin: 0 auto;
  margin-top: 70px;
  border: 1px solid #e8e8e8;
  vertical-align: middle;
}
/*.username input{
  border:none;
  outline: none;
}*/
.user{
  margin: 13px 10px 0 20px;
}
.user1{
  position: absolute;
  color: #5d5d5d;
  font-size: 16px;
}
.user2{
  border:none;
  outline: none;
  position: absolute;
  height: 50px;
  width: 300px;
  font-size: 16px;
  margin-left: 70px;
}
.password{
  height: 50px;
  width: 450px;
  line-height: 50px;
  margin: 0 auto;
  margin-top: 50px;
  border: 1px solid #e8e8e8;
}
.password input{
  border:none;
}
.key{
  margin: 13px 10px 0 20px;
}
.key1{
  position: absolute;
  color: #5d5d5d;
  font-size: 16px;  
}
.key2{
  border:none;
  outline: none;
  position: absolute;
  height: 50px;
  width: 300px;
  font-size: 16px;
  margin-left: 70px;
}
.remember{
  margin: 30px 0 0 43px;
}
.loginbtn{
  margin: 26px 0 0 43px;
}
.loginbtn1{
  width: 452px;
  height: 56px;
  font-size: 24px !important;
}
</style>
