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
  <RouterLink class="router" id="chesey" to="/">Shop</RouterLink>
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
#chesey {
  border: 1px solid black;
  left: 200px;
  width: 3rem;
  max-height: 3rem;
}
#chese {
  border: 1px solid black;
  justify-content: space-evenly;
  width: 3rem;
  max-height: 3rem;
}
</style>
