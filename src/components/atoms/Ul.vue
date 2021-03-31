<template>
  <ul>
    <slot />
  </ul>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({

})
</script>

<style scoped>
ul {
  /* list-style-type: none; */
  padding-left: 20px;
}
</style>
