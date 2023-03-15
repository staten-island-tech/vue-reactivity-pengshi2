<script>
import storeInventory from "../components/storeInventory.vue";

export default {
  components: {
    storeInventory,
  },
};
</script>

<template>
  <li v-for="item in items">
    {{ item.name }}
  </li>
</template>

<style></style>
