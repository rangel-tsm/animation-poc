<template>
  <q-list bordered class="rounded-borders full-width">
    <div v-for="(item, index) in listItems" :key="index">
      <q-expansion-item
        expand-separator
        :label="item.label"
      >
        <q-card bordered>
          <q-card-section>
            {{ item.description }}
          </q-card-section>
        </q-card>
      </q-expansion-item>
    </div>
  </q-list>
</template>

<script setup>
import { defineProps } from 'vue'

const props = defineProps({
  listItems: {
    type: Array,
    default: () => ([
      {
        label: "Test Label",
        description: "Description Text"
      }
    ])
  }
})
</script>

<style scoped>

</style>
