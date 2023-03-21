<script>
import items from "../components/items.js";
import storeInventory from "../components/things/storeInventory.vue";
export default {
  name: "HomeView",
  components: {},
  data() {
    return {
      items: items,
    };
  },
};
</script>

<template>
  <div class="home">
    <div class="storeCards">
      <storeInventory v-for="item in items" :key="item.id" :item="item" />
    </div>
  </div>
</template>

<style>
.storeCards {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
</style>
