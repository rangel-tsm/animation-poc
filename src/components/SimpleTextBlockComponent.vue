<template>
  <q-card>
    <q-card-section>
      <div class="text-h2">{{ title }}</div>
    </q-card-section>
    <q-card-section>
      <div v-if="expandedText">{{ expandedText }}</div>
      <slot></slot>
    </q-card-section>
  </q-card>
</template>

<script setup>
import { defineProps } from 'vue'

defineProps({
  expandedText: String,
  title: {
    type: String,
    required: true
  }
})
</script>

<style scoped>

</style>
