<template>
  <div class="news">
    <div class="news__container">
      <div class="news__title">
        Наши новости
        <div class="news__buttons">
          <button ref="prev" class="news__prev">
            <svg
              viewBox="0 0 8 14"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M7 13L1 7L7 1"
                stroke="#FF0000"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </button>
          <button ref="next" class="news__next">
            <svg
              viewBox="0 0 8 14"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M7 13L1 7L7 1"
                stroke="#FF0000"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </button>
        </div>
      </div>
      <div class="news__swiper">
        <Swiper
          :navigation="{
            prevEl: prev,
            nextEl: next,
          }"
          :slides-per-view="2"
          :space-between="40"
          :loop="true"
          :modules="modules"
        >
          <SwiperSlide>
            <img
              src="@/assets/img/news/materialy_elbrus_tech_day.png"
              alt=""
            /> </SwiperSlide
          ><SwiperSlide>
            <img
              src="@/assets/img/news/materialy_elbrus_tech_day.png"
              alt=""
            /> </SwiperSlide
        ></Swiper>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.news {
  margin-top: 8rem;
  &__next {
    svg {
      transform: rotate(180deg);
    }
  }
  &__buttons {
    display: flex;
    gap: 1.6rem;
    button {
      cursor: pointer;
      display: flex;
      align-items: center;
      justify-content: center;
      background-color: white;
      border: none;
      border-radius: 50%;
      padding: 1.2rem;
      box-shadow: 0px 8px 16px rgba(0, 0, 0, 0.16);
    }
    svg {
      width: 2.4rem;
      height: 2.4rem;
    }
  }
  &__title {
    font-size: 2.4rem;
    font-weight: bold;
    margin-bottom: 3rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  &__swiper {
  }
}
</style>

<script>
import { ref } from "vue";
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
    const prev = ref(null);
    const next = ref(null);
    return {
      modules: [Navigation, Pagination],
      prev,
      next,
    };
  },
};
</script>
