<template>
  <Ul>
    <li>{{ history.name }}</li>
    <Ul>
      <li>{{ history.description }}</li>
      <li>{{ history.date.start }} ~ {{ history.date.end }}</li>
    </Ul>
  </Ul>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import Ul from '../atoms/Ul.vue'

export default defineComponent({
  components: {
    Ul,
  },
  props: {
    history: {
      type: Object,
      required: true,
    },
  },
})
</script>
