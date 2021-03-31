<template>
  <div id="history">
    <H2>履歴</H2>
    <WorkHistory
      v-for="work in workHistory"
      :key="work.name"
      :history="work"
    />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { workHistory } from '../../data/history'
import H2 from '../atoms/H2.vue'
import WorkHistory from '../molecules/WorkHistory.vue'

export default defineComponent({
  components: {
    H2,
    WorkHistory,
  },
  setup () {
    return { workHistory }
  },
})
</script>
