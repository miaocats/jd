<template>
    <div class="homenew">
        <div class="main">-新手特权-</div>
        <div class="hmain">
        <div class='hcontent'>
            <p>下载app<span class="red">送888元礼包</span></p>
            <div class="small">新手专享</div>
            <img src="http://img12.360buyimg.com/jrpmobile/jfs/t10384/155/1759179594/9776/185bd062/59e5f0ebNec4cf494.png?width=100&height=100"/>
        </div>
        <div class='hcontent'>
            <p><span class="red">领128元新手...</span></p>
            <div class="small">新手专享 . . . . .</div>
            <img src="//img12.360buyimg.com/jrpmobile/jfs/t4639/162/1782623297/60754/98ea03b4/58e60952N7fdb2b85.png?width=200&height=200"/>
        </div>
        <div class='hcontent'>
            <p>打白条<span class="red">享免息</span></p>
            <div class="small">立即开通享豪礼</div>
            <img src="//img12.360buyimg.com/jrpmobile/jfs/t4804/179/657713323/5908/66dce262/58e6095fNd3dc3f39.png?width=100&height=100"/>
        </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'HomeNew'
}
</script>

<style lang="scss" scoped>
@import "../../assets/scss/element.scss";
.homenew{
    position: relative;
    background-color: #fff;
    padding-top: 10px;
    top: 10px;
    height: auto;
}
.main{
    display: flex;
    height: 42.37px;
    justify-content: center;
    align-items: center;
    font-size: 16px;
}
.hmain{
    display: flex;
    height: 145px;
    flex-direction: column;
    flex-wrap: wrap;
}
.hcontent{
    &:nth-child(1){
        display: flex;
        width: 50%;
        flex: 0 0 100%;
        flex-direction: column;
        justify-content: center;
        img{
            width: 66px;
            width: 66px;
            padding-top: 10px;
            align-self: center;
        }
    }
    &:nth-child(2){
        flex: 0 0 50%;
        width: 50%;
        p{
            float: left;
        }
        .small{
            float: left;
        }
    }
    &:nth-child(3){
        flex: 0 0 50%;
        width: 50%;
        p{
            float: left;
        }
        .small{
            float: left;
        }
    }
}
.small{
    font-size: 12px;
    color: grey;
    text-align: center;
    padding-top: 8px;

}
p{
    font-size: 13px;
    text-align: center;
    padding-top: 10px;
}
.red{
    color: red;
}
img{
    width: 30px;
    float: right;
}
</style>
