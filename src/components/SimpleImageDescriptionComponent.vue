<template>
  <q-card>
    <img :src="imageSrc" :alt="imageAlt"/>
    <q-card-section>
      <div class="text-h6">{{title}}</div>
      <div v-if="subtitle" class="text-subtitle2">{{ subtitle }}</div>
    </q-card-section>

    <q-card-section class="q-pt-none">
      {{ description }}
    </q-card-section>
  </q-card>
</template>

<script setup>
import { defineProps } from 'vue'

const props = defineProps({
  description: {
    type: String,
    required: true
  },
  imageAlt: {
    type: String,
    required: true
  },
  imageSrc: {
    type: String,
    required: true
  },
  title: {
    type: String,
    required: true
  },
  subtitle: {
    type: String
  }
})
</script>

<style scoped>

</style>
