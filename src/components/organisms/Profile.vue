<template>
  <div id="profile">
    <H2>私について</H2>
    <Ul>
      <li>名前: えむなお</li>
      <li>各ID: /^mnao_?305(#0355)?$/</li>
      <!-- 他に書く事無いんか??? -->
    </Ul>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import Ul from '../atoms/Ul.vue'
import H2 from '../atoms/H2.vue'

export default defineComponent({
  components: {
    H2,
    Ul,
  },
})
</script>
