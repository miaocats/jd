<template>
    <div>
        <div class="titles"><p class="title">-新品推荐-<span class='inside'>更多尖货</span></p>
        </div>
        <swiper :options="swiperOption">
    <swiper-slide v-for="(slide, index) in swiperSlides" :key="index">
      <img :src='slide.imgUrl'/>
      </swiper-slide>
    <div class="swiper-pagination" slot="pagination"></div>
  </swiper>
    </div>
</template>

<script>
import { swiper, swiperSlide } from 'vue-awesome-swiper'
export default {
  name: 'HomeProduct',
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
        slidesPerView: 3,
        spaceBetween: 30
      },
      swiperSlides: [{
        imgUrl: '//img12.360buyimg.com/jrpmobile/jfs/t13963/267/2355123229/48850/254f797a/5a3c59aeN9cb550f6.jpg?width=335&height=421'
      }, {
        imgUrl: '//img12.360buyimg.com/jrpmobile/jfs/t13021/306/1996997425/21953/bda69db3/5a2f6a17N9da099b1.jpg?width=335&height=421'
      }, {
        imgUrl: '//img12.360buyimg.com/jrpmobile/jfs/t14125/310/1997192193/46667/3c910f8b/5a2f6a36Nad95b650.jpg?width=335&height=421'
      }, {
        imgUrl: '//img12.360buyimg.com/jrpmobile/jfs/t15784/188/381232069/39444/8878571d/5a2f6a4aNbd5a574c.jpg?width=335&height=421'
      }]
    }
  }
}
</script>

<style lang="scss" scoped>
@import '../../assets/scss/element.scss';
@import '~swiper/dist/css/swiper.css';

.title{
    display: flex;
    height: 56px;
    justify-content: center;
    align-items: center;

}
.title{
    background-color: #fff;
}
.inside{
    position: absolute;
    right: 20PX;
}
img{
    height: 158px;
}

</style>
