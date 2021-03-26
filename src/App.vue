<template>
  <Profile />
  <Links />
  <Products />
  <History />
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import Profile from "./components/organisms/profile.vue";
import Links from "./components/organisms/links.vue";
import Products from "./components/organisms/products.vue";
import History from "./components/organisms/history.vue";

export default defineComponent({
  name: 'App',
  components: {
    Profile,
    Links,
    Products,
    History
  }
})
</script>
