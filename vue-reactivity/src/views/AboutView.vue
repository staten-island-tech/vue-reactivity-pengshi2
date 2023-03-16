<script>
import storeInventory from "../components/storeInventory.vue";

export default {
  components: {
    storeInventory,
  },
};
</script>

<template>
  <li v-for="item in list">
    {{ item.name }}
  </li>
</template>

<style></style>
