<template>
  <header>
    <H1>えむなお(mnao305)</H1>
  </header>
  <main>
    <Profile />
    <Links />
    <Products />
    <History />
  </main>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import Profile from './components/organisms/Profile.vue'
import Links from './components/organisms/Links.vue'
import Products from './components/organisms/Products.vue'
import History from './components/organisms/History.vue'
import H1 from './components/atoms/H1.vue'

export default defineComponent({
  name: 'App',
  components: {
    Profile,
    Links,
    Products,
    History,
    H1,
  },
})
</script>

<style>
html {
  background: #fafafa;
  font-size: 14px;
}

body {
  max-width: 700px;
  margin: 0 auto;
  padding: 0 10px;
}
</style>
