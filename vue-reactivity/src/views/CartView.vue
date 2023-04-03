<template>
  <div>
    <h1>Here is your shopping cart so far!</h1>
    <div class="cart">{{ store }}</div>
  </div>
</template>

<script>
import { store } from "../components/store.js";
import storeInventory from "../components/storeInventory.vue";
export default {
  data() {
    return {
      store,
      cart: [],
    };
  },
  props: { items: String },
};
</script>

<style>
font-family: "Delicious Handrawn", cursive;
</style>
