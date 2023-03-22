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
  <header>
    <div class="wrapper">
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style>
html,
body {
  margin: 0;
  padding: 0;
}
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}
</style>
