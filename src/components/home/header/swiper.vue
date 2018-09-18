<template>
  <div class="wrap">
    <swiper :options="swiperOption">
      <!-- slides -->
      <swiper-slide v-for="item in swiperSlides" :key="item.id">
        <img class="swipe-img" :src="item.imgUrl" alt="去哪儿门票" style="opacity: 1;">
      </swiper-slide>
      
      <!-- Optional controls -->
      <div class="swiper-pagination"  slot="pagination"></div>
      <!-- <div class="swiper-button-prev" slot="button-prev"></div>
      <div class="swiper-button-next" slot="button-next"></div>
      <div class="swiper-scrollbar"   slot="scrollbar"></div> -->
    </swiper>
  </div>
</template>

<script>
export default {
    data() {
      return {
        swiperOption:{
          pagination: '.swiper-pagination',
          loop:true
        },
        swiperSlides:[
          {id: '001',imgUrl:'http://img1.qunarzz.com/piao/fusion/1809/6a/847ac7b98f10e202.jpg_750x200_f0593cb5.jpg'},
          {id: '002',imgUrl:'http://img1.qunarzz.com/piao/fusion/1801/bd/04554e7c67650302.jpg_750x200_4293d60a.jpg'},
          {id: '003',imgUrl:'http://img1.qunarzz.com/piao/fusion/1808/f4/5f2289f8675f0502.jpg_750x200_ab1633c7.jpg'},
          {id: '004',imgUrl:'http://img1.qunarzz.com/piao/fusion/1806/1c/4847ea66072c7b02.jpg_750x200_c32457fb.jpg'},
          {id: '005',imgUrl:'http://img1.qunarzz.com/piao/fusion/1809/9b/8f79dbd1e0941302.jpg_750x200_55829659.jpg'},
          {id: '006',imgUrl:'http://img1.qunarzz.com/piao/fusion/1808/70/5603e6a535062402.jpg_750x200_2c552f2c.jpg'},
          {id: '007',imgUrl:'http://img1.qunarzz.com/piao/fusion/1809/50/670c61165170f902.jpg_750x200_c4b8d1dc.jpg'},
        ]
      }
    }
}
</script>

<style lang="stylus" scoped>
  .wrap >>> .swiper-pagination-bullet-active // >>> 表示穿透
      background #ffffff
  .wrap
    overflow hidden  
    width 100%
    height 0
    padding-bottom 26.67%
    .swipe-img
      width 100%
    
</style>