<template>
  <div class="login">
    <div class="login-form">
      <div class="login-form-block">
        <div class="login-form-block-top-center">
          <a href="#" class="jftj"></a>
          <a href="#" class="rmfy"></a>
        </div>
        <div class="login-form-block-top-center">
          <a href="#" class="fldjt"></a>
        </div>
      </div>
      <div class="login-form-block">
        <a href="#" class="lszx"></a>
        <a href="#" class="fdsf"></a>
      </div>
      <div class="login-form-block">
        <div class="login-form-block-bottom-top">
          <a href="#" class="grzx"></a>
        </div>
        <div class="login-form-block-bottom-bottom">
          <a href="#" class="weather"></a>
          <a href="#" class="set"></a>
        </div>     
      </div>     
    </div>  
  </div>
</template>
<script>
import { getCodeImg } from "@/api/login";
import Cookies from "js-cookie";
import { encrypt, decrypt } from '@/utils/jsencrypt'

export default {
  name: "Login",
  data() {
    return {
     
    }
  } 
};
</script>

<style rel="stylesheet/scss" lang="scss">
.login-form-block{
  width:32%;
  float:left;
}
.login-form-block-bottom-bottom{
  margin-top:20px;
}
.jftj{
  display:inline-block;
  width:200px;
  height:200px;
  background-image: url("../assets/images/jftj.png");
  background-size:100% 100%;
  float:left;
  margin-right:15px;
}
.rmfy{
  display:inline-block;
  width:200px;
  height:200px;
  background-image: url("../assets/images/rmfy.png");
  background-size:100% 100%;
  float:left;
}
.fldjt{
  display:inline-block;
  width:410px;
  height:200px;
  background-image: url("../assets/images/fldjt.png");
  background-size:100% 100%;
  margin-top:20px;
}
.lszx{
  display:inline-block;
  width:410px;
  height:200px;
  background-image: url("../assets/images/lszx.png");
  background-size:100% 100%;
}
.fdsf{
  display:inline-block;
  width:410px;
  height:200px;
  background-image: url("../assets/images/fdsf.png");
  background-size:100% 100%;
  margin-top:20px;
}
.grzx{
  display:inline-block;
  width:410px;
  height:200px;
  background-image: url("../assets/images/grzx.png");
  background-size:100% 100%;
}
.weather{
  display:inline-block;
  width:200px;
  height:200px;
  background-image: url("../assets/images/weather.png");
  background-size:100% 100%;
  float:left;
  margin-right:15px;
}
.set{
  display:inline-block;
  width:200px;
  height:200px;
  background-image: url("../assets/images/set.png");
  background-size:100% 100%;
  float:left;
}
.login {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100%;
  background-image: url("../assets/images/bg.png");
  background-size: cover;
}
.title {
  margin: 0px auto 30px auto;
  text-align: center;
  color: #707070;
}

.login-form {
  border-radius: 6px;
  width: 86%;
  padding: 25px 25px 5px 25px;
  .el-input {
    height: 38px;
    input {
      height: 38px;
    }
  }
  .input-icon {
    height: 39px;
    width: 14px;
    margin-left: 2px;
  }
}
.login-tip {
  font-size: 13px;
  text-align: center;
  color: #bfbfbf;
}
.login-code {
  width: 33%;
  height: 38px;
  float: right;
  img {
    cursor: pointer;
    vertical-align: middle;
  }
}
.el-login-footer {
  height: 40px;
  line-height: 40px;
  position: fixed;
  bottom: 0;
  width: 100%;
  text-align: center;
  color: #fff;
  font-family: Arial;
  font-size: 12px;
  letter-spacing: 1px;
}
.login-code-img {
  height: 38px;
}
</style>
