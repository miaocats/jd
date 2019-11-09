<template>
    <section :class="cname">
        <swiper :options="swiperOption" :not-next-tick="swiperOptions.notNextTick">
            <swiper-slide v-for="item in items" :key="item.href">
                <router-link :to="{name:item.href}"><img :src="item.src" alt=""></router-link>
            </swiper-slide>
            <div class="swiper-pagination" v-if="swiperOption.pagination"/>
        </swiper>
    </section>
</template>

<script>
import { swiper, swiperSlide } from 'vue-awesome-swiper'
export default {
  components: {
    swiper,
    swiperSlide
  },
  props: {
    swiperOption: {
      type: Object,
      default () {
        return {
          autoplay: true,
          loop: true,
          pagination: {
            el: '.swiper-pagination'
          },
          notNextTick: false
        }
      }
    },
    items: {
      yoe: Object,
      default () {
        return []
      }
    }
  }
}
</script>

<style lang="scss">
@import '~swiper/dist/css/swiper.css';
@import "../../assets/scss/element.scss";
.panel{
    @include panel;
}
</style>
