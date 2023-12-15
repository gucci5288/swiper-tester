<template>
  <div class="about">
    <h1>This is an swiper page</h1>
    <swiper
        :speed="1000"
    >
      <swiper-slide
        v-for="i in 5" :key="i"
      >
        <test-content/>
      </swiper-slide>
    </swiper>
  </div>
</template>

<script setup lang="ts">
import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/css';

import TestContent from "@/components/icons/TestContent.vue";

</script>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
