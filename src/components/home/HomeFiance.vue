<template>
    <div>
        <div class='title'>-理财精选-</div>
        <div class="list">
            <div class='item'>
                <h4>定期理财</h4>
                <div class='red'>5.60%</div>
                <p>历史年回报率</p>
            </div>
            <div class='item'>
                <h4>小白理财</h4>
                <div class='red'>4.22%</div>
                <p>7日年华收益率</p>
            </div>
            <div class='item'>
                <h4>月月盈</h4>
                <div class='red'>5.6%</div>
                <p>历史年回报率</p>
            </div>
            <div class='item'>
                <h4>小白基金</h4>
                <div class='red'>5.6%</div>
                <p>历史年回报率</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'HomeFiance'
}
</script>

<style lang="scss" scoped>
@import '../../assets/scss/element.scss';
.title{
    @include panel;
    display: flex;
    height: 56px;
    justify-content: center;
    align-items: center;
}
.list{
    display: flex;
    flex-wrap: wrap;
    flex-direction: row;
}
.item{
    flex: 0 0 50%;
    height: 101.9px;
}
h4{
    font-size: 15px;
    padding-left: 10px;
}
.red{
    font-size: 22px;
    color: red;
    padding-top: 10px;
    padding-left: 10px;
}
p{
    font-size: 12px;
    padding-top: 10px;
    padding-left: 10px;
}
</style>
