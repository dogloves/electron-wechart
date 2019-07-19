<template>
  <div class="login-wrap">
    <div class="logo"><img src=""></div>
    <div class="form-box">
      <div class="form-phone form-item">
        <div class="phone-bofore">{{phoneBefore}}</div>
        <div class="sel-icon"><i class="el-icon-arrow-down"></i></div>
        <div class="line">|</div>
        <input type="text" placeholder="请输入手机号">
      </div>
      <div class="form-psd form-item">
        <input type="password" placeholder="请输入密码">
      </div>
      <div class="query-btn">登录</div>
    </div>

    <div class="btm-box">
      <div class="btm-item">忘记密码</div>
      <div class="line">|</div>
      <div class="btm-item">新用户注册</div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'login',
  data () {
    return {
      phoneBefore: '+86'
    };
  },
  methods: {

  },
};
</script>

<style scoped lang="scss">
.login-wrap {
  width: 100%;
  height: 100%;
  flex-direction: column;
  display: flex;
  align-items: center;
  justify-content: center;
  .logo {
    width: 115px;
    height: 100px;
    background: red;
  }
  .form-box {
    width: 240px;
    margin-top: 40px;
  }
  .form-item {
    width: 100%;
    height: 45px;
    border-bottom: 1px solid #555;
    padding-top: 10px;
    line-height: 30px;
  }
  .form-phone {
    display: flex;
    .phone-bofore {
      padding: 0 10px;
      cursor: pointer;
    }
    .line {
      padding: 0 5px;
    }
  }
  input {
    width: 160px;
    height: 30px;
    border: none;
    outline: none;
    padding-left: 15px;
  }
  .query-btn {
    width: 140px;
    height: 40px;
    margin: auto;
    margin-top: 30px;
    border: 1px solid #777;
    border-radius: 5px;
    line-height: 40px;
    text-align: center;
    cursor: pointer;
  }
  .btm-box {
    display: flex;
    justify-content: flex-end;
    position: absolute;
    right: 20px;
    bottom: 10px;
    font-size: 13px;
    color: #777;
    line-height: 30px;
    .btm-item {
      padding: 0 5px;
      cursor: pointer;
    }
  }
}
</style>
