<script>
export default {
  data() {
    return {};
  },
  components: {},
};
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header class="header">CSGO SKINS</header>
  <RouterLink class="router" id="chese" to="/">Shop</RouterLink>
  <RouterLink class="router" id="chese" to="/cart">View Cart</RouterLink>
  <RouterView />
</template>

<style>
.header {
  text-align: center;
  font-size: 40px;
  left: 100px;
  border: 1px solid black;
}

.router {
  size: 50%;
}

#chese {
  justify-content: space-evenly;
  width: 5rem;
  max-height: 5rem;
}
</style>
