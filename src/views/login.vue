<template>
  <div class="contain">
    <div class="TitleBox">
      <div class="TitleHead">跨境营销服务平台</div>
      <div class="TitleTip">让行业没有难做的跨境电商</div>
      <div class="LoginBgIcon"></div>
    </div>
    <div class="LoginBox" :class="{active:isLogin}">
      <div class="title">Demo</div>
      <div class="LoginForm">
        <input type="text" class="LoginInput" placeholder="请输入用户名" v-model="form.username">
        <input type="password" class="LoginInput" placeholder="请输入密码" v-model="form.userpwd">
        <button @click="login">登录</button>
        <div class="BtmTip">登录即视为同意 <i>《用户协议》</i></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'contain',
  data () {
    return {
      isLogin: false,
      login: false,
      form: {
        username: '',
        userpwd: ''
      }
    }
  }
}
</script>

<style scoped>
.TitleBox{
  text-align: left;
  margin: 8% 10%;
  float: left;
  width: 440px;
}

.TitleHead{
  color: #006CCC;
  font-size: 50px;
  letter-spacing: 5px;
  font-weight: bold;

}
.TitleTip{
  color: #9E9E9E;
  font-size: 14px;
  text-align: center;
  margin: 10px;
  letter-spacing: 10px;
}
.LoginBgIcon{
  height: 680px;
  width: 700px;
  background: url("../assets/phone-web-icon-all.png") no-repeat;
  background-size: 100%;
}
.LoginBox{
  height: 420px;
  width: 450px;
  float: right;
  background: #ffffff;
  border-radius: 10px;
  position: absolute;
  top: 30%;
  right: 15%;
  box-shadow: 0 0 50px #ece9e9
}
.title{
  font-size: 30px ;
  margin-top: 20px;
  font-weight: bold;
  letter-spacing: 10px;
  color: #006CCC;
  text-align: center;
}

.LoginForm{
  margin-top: 35px;
}

.LoginForm .LoginInput{
  width: 80%;
  height: 40px;
  margin: 15px;
  border-radius: 5px;
  border:1px solid  #D1D1D1;
  padding:5px 20px;
  text-align: left;
  font-size: 16px;
}
.LoginForm button{
  width: 90%;
  height: 65px;
  border-radius: 10px;
  background: #509FFF;
  border: none;
  text-align: center;
  letter-spacing: 10px;
  color: white;
  font-size: 20px;
  margin-top: 30px;
  cursor: pointer;
}
.BtmTip{
  font-size: 14px;
  margin-top:20px;
  text-align: center;
}
.BtmTip i{
font-style: normal;
  color: #006CCC;
  cursor: pointer;
}
</style>
