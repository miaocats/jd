<template>
    <div><h4 class='title'>-生活服务-</h4>
    <div class="hicons">
        <div class="icon" v-for='(item,index) in items' :key='index'>
            <img class="img" :src="item.url"/>
            <p class="txt">{{item.name}}</p>
        </div>
    </div>
    <img  class='banner' src='//img12.360buyimg.com/jrpmobile/jfs/t2842/350/3035567089/14791/5f6ff93d/577cf395N31e76288.png?width=1125&height=252'/>
    </div>

</template>

<script>
export default {
  name: 'HomeLife',
  data () {
    return { items: [{
      name: '惠加油',
      url: '//img12.360buyimg.com/jrpmobile/jfs/t4375/104/1184122472/3976/89741da4/58be8a6eNf10193d0.png?width=135&height=135'
    }, {
      name: '小白信用',
      url: '//img12.360buyimg.com/jrpmobile/jfs/t4747/185/1901740991/5892/1383fb93/58f57851N17ee6993.jpg?width=132&height=132'
    }, {
      name: '信用卡还...',
      url: '//img12.360buyimg.com/jrpmobile/jfs/t3241/234/8044685271/3713/7b29f77f/58be89c8Nb9d41295.png?width=135&height=135'
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
@import '../../assets/scss/element.scss';
.title{
    @include panel;
    height: 56px;
    display: flex;
    justify-content: center;
    align-items: center;
}
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
.banner{
  height: 70px;
  width: 100%;
}
</style>
