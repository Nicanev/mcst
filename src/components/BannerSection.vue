<template>
  <section class="banner">
    <Swiper
      :slides-per-view="1"
      :pagination="{
        clickable: true,
        el: '.banner__pagination',
      }"
      :loop="true"
      :modules="modules"
    >
      <SwiperSlide>
        <img src="@/assets/img/banners/maxresdefault.jpg" alt="" />
      </SwiperSlide>
      <SwiperSlide>
        <img src="@/assets/img/banners/maxresdefault.jpg" alt="" />
      </SwiperSlide>
      <div class="banner__pagination"></div>
    </Swiper>
  </section>
</template>

<style lang="scss">
.banner {
  img {
    width: 100%;
    height: 77rem;
  }
  &__pagination {
    position: relative;
    text-align: center;
    margin-top: -2rem;
    z-index: 100;
  }
  .swiper-pagination-bullet-active {
    background-color: white !important;
    border: 0.2rem solid black;
  }
}
</style>

<script>
import { Swiper, SwiperSlide } from "swiper/vue";
import "swiper/css";
import { Navigation, Pagination } from "swiper";
import "swiper/css/pagination";
export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Navigation, Pagination],
    };
  },
};
</script>
