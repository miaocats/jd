<template>
  <div>
    <home-header></home-header>
    <home-swiper></home-swiper>
    <home-icons></home-icons>
    <home-new></home-new>
    <home-borrow></home-borrow>
    <home-fiance></home-fiance>
    <home-product></home-product>
    <home-life></home-life>
    <home-tail></home-tail>
    <home-button></home-button>
  </div>
</template>

<script>
import HomeHeader from '@/components/home/HomeHeader.vue'
import HomeSwiper from '@/components/home/HomeSwiper.vue'
import HomeIcons from '@/components/home/HomeIcons.vue'
import HomeNew from '@/components/home/HomeNew.vue'
import HomeBorrow from '@/components/home/HomeBorrow.vue'
import HomeFiance from '@/components/home/HomeFiance.vue'
import HomeProduct from '@/components/home/HomeProduct.vue'
import HomeLife from '@/components/home/HomeLife.vue'
import HomeTail from '@/components/home/HomeTail.vue'
import HomeButton from '@/components/home/HomeButton.vue'

export default {
  name: 'home',
  components: {
    HomeHeader,
    HomeSwiper,
    HomeIcons,
    HomeNew,
    HomeBorrow,
    HomeFiance,
    HomeProduct,
    HomeLife,
    HomeTail,
    HomeButton
  }
}
</script>
