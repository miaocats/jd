<template>
<div class=".headers">
    <div class='header'>
        <div class='text'>注册 | 登录
        </div>
        <btn class='hbtn'>app下载
        </btn>
    </div>
    </div>
</template>

<script>
import btn from '../core/btn.vue'
export default {
  name: 'HomeHeader',
  components: {
    btn
  }
}
</script>

<style lang="scss" scoped>
@import "../../assets/scss/element.scss";
.headers{
  position: fixed;
  z-index: 999;
}
.header{
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 50px;
  background: #fff url(//m.jr.jd.com/spe/qyy/main/images/jr-logo.png) center center no-repeat;
  background-size: auto 50%;
  margin-bottom: 10px;
}
.text{
  font-size: 14px;
  padding-left: 10px;
  }
.hbtn{
  margin-right: 15px;
  }
</style>
