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
  <header class="header">CSGO SKINS</header>
  <RouterLink class="router" id="chese" to="/">Home</RouterLink>
  <RouterLink class="router" id="chese" to="/cart">View Cart</RouterLink>
  <RouterView />
</template>

<style>
.header {
  text-align: center;
  font-size: 50px;
  left: 50px;
}

.router {
  size: 50%;
}

#chese {
  width: 5rem;
  max-height: 5rem;
}
</style>
