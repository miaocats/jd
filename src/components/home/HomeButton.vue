<template>
    <div>
      <div class='buttons'>
        <div class='button'>
        <img src='//img12.360buyimg.com/jrpmobile/jfs/t3451/188/644771475/2428/800d7cb7/580f2435Nbfaa8055.png?width=66&height=66'/>
        <a>首页</a>
        </div>
        <div class='button'>
        <img src='//img12.360buyimg.com/jrpmobile/jfs/t3811/55/345433999/2930/116d3dd1/580f1e25N028a1f2c.png?width=66&height=66'/>
        <a>理财</a>
        </div>
        <div class='button'>
        <img src='//img12.360buyimg.com/jrpmobile/jfs/t3343/179/621044750/1484/5af6b11a/580f50e4N005181d0.png?width=66&height=66'/>
        <a>白条</a>
        </div>
        <div class='button'>
        <img src='//img12.360buyimg.com/jrpmobile/jfs/t3604/98/635506544/2317/443d3a51/580f240aNbee3dcc4.png?width=66&height=66'/>
        <a>众筹</a>
        </div>
        <div class='button'>
        <img src='//img12.360buyimg.com/jrpmobile/jfs/t3340/68/639059082/2591/800e2d6b/580f51cdN4caf20b2.png?width=66&height=66'/>
        <a>我的</a>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: 'HomeButton'
}
</script>

<style lang="scss" scoped>
.buttons{
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  background-color: #fff;
}
.button{
  display: flex;
  flex-direction: column;
  img{
    width: 22px;
  }
  a{
    font-size: 11px;
  }
  a:active{
    color:red;
  }
  a:visited{
    color: red;
  }
}
</style>
