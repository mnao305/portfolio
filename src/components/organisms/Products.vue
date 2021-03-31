<template>
  <div id="products">
    <H2>作ったもの</H2>
    <Product
      v-for="product in products"
      :key="product.name"
      :product="product"
    />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { products } from '../../data/products'
import H2 from '../atoms/H2.vue'
import Product from '../molecules/Product.vue'

export default defineComponent({
  components: {
    H2,
    Product,
  },
  setup () {
    return { products }
  },
})
</script>
