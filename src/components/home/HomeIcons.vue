<template>
    <div class="hicons">
        <div class="icon" v-for='(item,index) in items' :key='index'>
            <img class="img" :src="item.url"/>
            <p class="txt">{{item.name}}</p>
        </div>
    </div>
</template>

<script>
export default {
  name: 'HomeIcons',
  data () {
    return { items: [{
      name: '优惠券',
      url: '//img12.360buyimg.com/jrpmobile/jfs/t3991/64/2521945388/12110/93c0139/58d1e462Ncf294123.png?width=132&height=132'
    }, {
      name: '领红包',
      url: '//img12.360buyimg.com/jrpmobile/jfs/t5590/252/875247023/17343/946aa72c/59224650N0f7ffc92.png?width=132&height=132'
    }, {
      name: '抢钢镚',
      url: '//img12.360buyimg.com/jrpmobile/jfs/t4618/115/2179710654/11347/bf520df/58ec9d84Nfd169001.png?width=132&height=132'
    }, {
      name: '领京豆',
      url: '//img12.360buyimg.com/jrpmobile/jfs/t4618/115/2179710654/11347/bf520df/58ec9d84Nfd169001.png?width=132&height=132'
    }, {
      name: '白条提额',
      url: '//img12.360buyimg.com/jrpmobile/jfs/t5488/298/1036263348/12073/b4f4de97/590ac8e8Ne9def22e.png?width=135&height=135'
    }]
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../../assets/scss/element.scss";
.hicons{
    display: flex;
    flex-direction: row;
    height: 95.8px;
    justify-content: space-around;
    align-items: center;
    background-color: #fff;
}
.icons{
    width: 10%;
}
.img{
    width: 45px;
    height: 45px;
}
.txt{
    font-size: 13px;
    color: #666;
}
</style>
