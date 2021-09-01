<template>
  <div class="main">
    <div class="empty"></div>
    <div class="card">
      <div class="left_empty"></div>
      <el-card class="box-card">
        <div class="title_parent">
          <div class="title">
            <p class="text">vue实训系统</p>
          </div>
          <div class="float">
          </div>
        </div>
        <div class="form">
          <el-form :model="ruleForm"
                   status-icon
                   :rules="rules"
                   ref="ruleForm"
                   class="demo-ruleForm">
            <el-input placeholder="请输入账号"></el-input>
            <el-input type="password"
                      autocomplete="off"
                      placeholder="请输入密码"></el-input>
          </el-form>
          <el-button type="primary">提交</el-button>
          <el-button type="primary" style="margin-left:0px">提交</el-button>
        </div>
      </el-card>
    </div>
    <div class="empty"></div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
.item {
  padding: 20px 0;
}
.card {
  width: 100%;
}
.box-card {
  width: 400px;
  height: 500px;
  margin: 0 auto;
}
.el-form {
  margin-top: 200px;
}
.el-input {
  margin-bottom: 20px;
}
.empty {
  height: 120px;
}
.title {
  position: relative;
  top: 0;
  margin-left: -50px;
  background-color: rgb(0, 128, 111);
  height: 70px;
  width: 400px;
  margin-top: 100px;
}
.title_parent {
  position: absolute;
}
.text {
  line-height: 65px;
  color: aliceblue;
  margin-left: 30px;
}
.float {
  width: 0;
  height: 0;
  border-top: 20px solid rgb(0, 0, 0);
  border-left: 30px solid transparent;
  margin-left: -50px;
}
.el-button{
  width: 360px;
  margin-bottom: 20px;
  background-color: rgb(0, 128, 111);
}
</style>
