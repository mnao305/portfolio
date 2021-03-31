<template>
  <div id="links">
    <H2>リンク</H2>
    <Ul>
      <li
        v-for="link in links"
        :key="link.name"
      >
        <A
          :href="link.url"
          target="_blank"
        >
          {{ link.name }}
        </A>
      </li>
    </Ul>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import H2 from '../atoms/H2.vue'
import Ul from '../atoms/Ul.vue'
import A from '../atoms/A.vue'
import { links } from '../../data/links'

export default defineComponent({
  components: {
    H2,
    Ul,
    A,
  },
  setup () {
    return { links }
  },
})
</script>
