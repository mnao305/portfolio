<template>
  <a :href="href"><slot /></a>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  props: {
    href: {
      type: String,
      required: true,
    },
  },
})
</script>

<style scoped>
a {
  color: #000;
}
a:hover {
  color: #22f;
}
</style>
