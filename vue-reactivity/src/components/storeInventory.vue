<template>
  <div class="coolcard">
    <h2>{{ name }}</h2>
    <h3 class="cost">$ {{ price }}</h3>
    <img :src="getImage" alt="" />
    <p class="Description">Description: {{ Description }}</p>
  </div>
</template>

<script>
export default {
  name: "storeInventory",
  props: {
    name: String,
    cost: Number,
    Description: String,
    image: String,
  },
  computed: {
    getImage: function () {
      return this.image;
    },
  },
};
</script>

<style scoped>
.coolcard {
  background-color: red;
}
</style>
