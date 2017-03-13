<template>
  <div class="loginbox">
    <div class="bginpputbox">
      <!--<h1>{{ msg }}</h1>-->
      <div class="logowrap">
        <div class="item"></div>
        <div class="item logo">
          <!--<img :src="LogoPath">-->
          <div class="logobox"></div>
        </div>
        <div class="item"></div>
      </div>
      <div class="inputbox">
        <div class="usernamebox">
          <div class="userlogobox">
            <span class="icon-user"></span>
          </div>
          <input type="text" class="inputfrom" placeholder="请输入登录账号">
        </div>
        <div class="usernamebox">
          <div class="userlogobox">
            <span class="icon-key"></span>
          </div>
          <input type="password" class="inputfrom" placeholder="请输入密码">
        </div>
        <div class="btnbox">
          <a class="loginbtn" href="javascript:">登录</a>
        </div>
      </div>
    </div>
    <footer>
        <a href="javascript:">忘记密码？</a>
        <a href="javascript:">新用户</a>
    </footer>
  </div>
</template>

<script type="text/ecmascript-6">
export default {
  name: 'Login',
  data () {
    return {
      msg: 'LOVE TO DO LIST!'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style  lang="sass" rel="stylesheet/sass">
  @import "../../common/sass/Color"
  @import "../../common/sass/mixin"
  @import "../../common/sass/widhth"
  .loginbox
    height: $hundred
    display: flex
    min-height: 100vh
    flex-direction: column
    .bginpputbox
      flex: 1
      .logowrap
        height: 36%
        display: flex
        .item
          flex-grow: 1
          height: 100%
        .logo
          @include screen
          flex-grow: 2
          display: flex
          justify-content: center
          align-items: center
          .logobox
            width: $hundred
            height: 50%
            background: url("logo.png")
            background-size: 100% 100%
      .inputbox
      .usernamebox
        width: $nine
        margin: 6% auto
        display: flex
        border-bottom: 1px solid $gray
        .userlogobox
          display: inline-block
          margin-top: 3px
          flex-shrink: 0
          span
            display: inline-block
            font-size: 30px
            color: $blue1
        .inputfrom
          width: $hundred
          padding: 10px
          border: 0
          background-color: $white
          outline: none
          vertical-align: top
      .btnbox
        text-align: center
        .loginbtn
          display: inline-block
          width: $nine
          @include margin-auto
          background: $blue1
          color: $white
          font-weight: bold
          font-size: 16px
          padding: 10px
          text-align: center
          border-radius: 6px
    footer
      width: $nine
      @include margin-auto
      padding: 0 10px 20px 10px
      display: flex
      justify-content: space-between


</style>
