<template>
  <div class="coolcard">
    <h2>{{ name }}</h2>
    <p class="price">${{ price }}</p>
    <br />
    <img :src="getImage" alt="" />
    <br />
    <p class="description">{{ description }}</p>
    <br />
    <p class="condition">Condition: {{ condition }}</p>
  </div>
</template>

<script>
export default {
  name: "storeInventory",
  props: {
    name: String,
    price: Number,
    description: String,
    image: String,
    condition: String,
  },
  computed: {
    getImage: function () {
      return this.image;
    },
  },
};
</script>

<style scoped></style>
