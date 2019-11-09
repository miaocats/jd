<template>
    <div>
        <div class='icons'>
            <div class='icon'>
                <img src='//img12.360buyimg.com/jrpmobile/jfs/t2971/333/1297567079/898/f2d2e00d/577dc28dNe5138337.png?width=108&height=108'/>
                <p>客户端</p>
            </div>
            <div class='icon'>
                <img src='http://img12.360buyimg.com/jrpmobile/jfs/t2824/256/2966087355/831/188bfa25/577cf3dcN18aadbf2.png?width=108&height=108'/>
                <p>触控板</p>
            </div>
            <div class='icon'>
                <img src='//img12.360buyimg.com/jrpmobile/jfs/t2920/282/1283157010/1040/23f1430b/577cf3e5N53f740b8.png?width=108&height=108'/>
            <p>电脑版</p>
            </div>
        </div>
        <div class="text">
            <li>Copyright © 2004-2017 京东JD.com 版权所有</li>
            <li>投资有风险，购买需谨慎</li>
            <li>京东金融平台服务协议</li>
        </div>
    </div>
</template>

<script>
export default {
  name: 'HomeTail'
}
</script>

<style lang='scss' scoped>
.icons{
    display: flex;
    flex-direction: row;
    flex: 0 0 100%;
    justify-content: space-around;
}
.icon{
    flex: 0 0 33.3333%;
    align-items: center;
    display: flex;
    justify-content: center;
    flex-direction: column;
    p{
        font-size: 12px;
    }
}
img{
    width: 45px;
}
.text{
    display: flex;
    flex-direction: column;
    justify-content: center;
    list-style: none;
    align-content: center;
    li{
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 12px;
        height: 40px;
    }
}
</style>
