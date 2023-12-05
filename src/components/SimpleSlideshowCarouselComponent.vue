<template>
  <div class="q-pa-md">
    <q-carousel
      animated
      v-model="slide"
      navigation
      infinite
      :autoplay="autoplay"
      arrows
      transition-prev="slide-right"
      transition-next="slide-left"
      @mouseenter="autoplay = false"
      @mouseleave="autoplay = true"
    >
      <q-carousel-slide v-for="(image, i) in images" :name="image.name" :img-src="image.url" :key="i"/>
    </q-carousel>
  </div>
</template>

<script setup>
import { defineProps, onMounted, ref } from 'vue';

const props = defineProps ({
  autoplayEnabled: {
    type: Boolean,
    default: () => false
  },
  images: {
    type: Array,
    required: true
  }
})
const slide = ref(1);
let autoplay = false;

onMounted(() => {
  if(props.autoplayEnabled) {
    autoplay = true
  }
})
</script>

<style scoped>

</style>
