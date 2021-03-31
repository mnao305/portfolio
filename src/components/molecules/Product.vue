<template>
  <Ul>
    <li>
      <A
        :href="product.url"
        target="_blank"
      >{{ product.name }}</A>
    </li>
    <Ul>
      <li>{{ product.description }}</li>
      <li>{{ product.tools }}</li>
    </Ul>
  </Ul>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import Ul from '../atoms/Ul.vue'
import A from '../atoms/A.vue'

export default defineComponent({
  components: {
    Ul,
    A,
  },
  props: {
    product: {
      type: Object,
      required: true,
    },
  },
})
</script>
