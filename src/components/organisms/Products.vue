<template>
  <div id="products">
    <H2>作ったもの</H2>
    <Ul>
      <Product
        v-for="product in products"
        :key="product.name"
        :product="product"
      />
      <li>
        その他
        <A
          href="https://github.com/mnao305?tab=repositories"
          target="_blank"
        >GitHub repository ページ</A>参照
      </li>
    </Ul>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { products } from '../../data/products'
import Product from '../molecules/Product.vue'
import H2 from '../atoms/H2.vue'
import A from '../atoms/A.vue'
import Ul from '../atoms/Ul.vue'

export default defineComponent({
  components: {
    H2,
    Product,
    Ul,
    A,
  },
  setup () {
    return { products }
  },
})
</script>
