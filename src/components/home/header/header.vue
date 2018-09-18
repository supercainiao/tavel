<template>
  <div class="header">
      <div class="header-left">
        <img src="./../../../assets/styles/icon/fanhui.png" alt="">
      </div>
      <div class="header-input">
        <img src="./../../../assets/styles/icon/sousou.png" alt="">
        输入城市/景点/游玩主题
      </div>
      <div class="header-right">
        城市
        <img src="./../../../assets/styles/icon/xiangxia.png" alt="">
      </div>
  </div>
</template>

<script>
export default {
    
}
</script>

<style lang="stylus" scoped>
@import '~@/assets/styles/variable.styl'
.header
  display flex
  line-height .86rem
  height: .86rem
  color #fff
  background $bgColor
  .header-left
    width .64rem
    float left
    img
      text-align center
      margin-left .15rem
  .header-input
    flex 1
    background #fff
    border-radius .1rem
    height .64rem
    margin .12rem .1rem .12rem .1rem
    line-height .64rem
    color #ccc
    img 
      padding-left .15rem
  .header-right
    width 1.24rem
    float right
    text-align center
    img 
      margin-left -0.04rem
</style>

