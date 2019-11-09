<template>
  <swiper :options="swiperOption">
    <swiper-slide v-for="(slide, index) in swiperSlides" :key="index">
      <img :src='slide.imgUrl'/>
      </swiper-slide>
    <div class="swiper-pagination" slot="pagination"></div>
  </swiper>
</template>

<script>
import { swiper, swiperSlide } from 'vue-awesome-swiper'

export default {
  name: 'HomeSwiper',
  components: {
    swiper,
    swiperSlide
  },
  data () {
    return {
      swiperOption: {
      // some swiper options/callbacks
      // 所有的参数同 swiper 官方 api 参数
      // ...
        pagination: '.swiper-pagination',
        loop: true
      },
      swiperSlides: [{
        imgUrl: '//img12.360buyimg.com/jrpmobile/jfs/t13744/11/2508939408/43213/58bfe502/5a421ff3N52d0a474.jpg?width=750&height=320'
      }, {
        imgUrl: '//img12.360buyimg.com/jrpmobile/jfs/t16138/325/817844900/36681/5d874455/5a422029Ncd678ea3.jpg?width=750&height=320'
      }, {
        imgUrl: '//img12.360buyimg.com/jrpmobile/jfs/t13465/324/2563794460/43029/3ffca963/5a421f83Ne8089231.jpg?width=750&height=320'
      }]
    }
  }
}
</script>

<style lang="scss" scoped>
@import '~swiper/dist/css/swiper.css';
img{
  height: 136.5px;
  width: 100%;
}
</style>
