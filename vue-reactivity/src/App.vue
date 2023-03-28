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
  <RouterLink to="/checkout">Checkout</RouterLink>
  <RouterView />
</template>

<style></style>
