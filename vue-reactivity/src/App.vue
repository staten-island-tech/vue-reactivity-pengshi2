<script>
export default {
  data() {
    return {};
  },
  components: { StoreInventory },
};
import { RouterLink, RouterView } from "vue-router";
import StoreInventory from "./components/storeInventory.vue";
</script>

<template>
  <RouterLink to="/">Home</RouterLink>
  <RouterLink to="/about">About</RouterLink>
  <RouterView />
</template>

<style>
html,
body {
  margin: 0;
  padding: 0;
  background-color: red;
}
</style>
