<template>
  <Profile />
  <Links />
  <Products />
  <History />
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import Profile from "./components/organisms/Profile.vue";
import Links from "./components/organisms/Links.vue";
import Products from "./components/organisms/Products.vue";
import History from "./components/organisms/History.vue";

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
