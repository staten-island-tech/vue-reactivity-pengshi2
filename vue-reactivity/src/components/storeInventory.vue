<template>
  <div class="coolcard">
    <br />
    <h2 class="name">{{ name }}</h2>
    <p class="price">${{ price }}</p>
    <br />
    <img :src="getImage" alt="" />
    <br />
    <h3 class="description">{{ description }}</h3>
    <br />
    <p class="condition">Condition: {{ condition }}</p>
    <br />
    <button v-on:click="addItemToCart(item)" class="buy">Add to Cart</button>
    <button v-on:click="" class="remove">Remove from Cart</button>
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

<style></style>
