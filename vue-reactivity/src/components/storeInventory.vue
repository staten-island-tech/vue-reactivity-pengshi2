<template>
  <div class="coolcard">
    <h2>{{ name }}</h2>
    <p class="cost">${{ price }}</p>
    <img :src="getImage" alt="" />
    <p class="description">{{ description }}</p>
    <p class="type">{{ type }}</p>
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
    type: String,
  },
  computed: {
    getImage: function () {
      return this.image;
    },
  },
};
</script>

<style scoped></style>
