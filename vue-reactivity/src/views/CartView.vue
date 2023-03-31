<template>
  <div>
    <h1>Here is your shopping cart so far!</h1>
  </div>
</template>

<script>
import storeInventory from "../components/storeInventory.vue";
export default {
  data() {
    return {
      cart: [],
    };
  },
};
</script>

<style>
font-family: "Delicious Handrawn", cursive;
</style>
