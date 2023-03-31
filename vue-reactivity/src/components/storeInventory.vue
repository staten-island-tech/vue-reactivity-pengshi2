<template>
  <div class="coolcard">
    <h2 class="name">{{ name }}</h2>
    <p class="price">${{ price }}</p>
    <img :src="getImage" alt="" />
    <h3 class="description">{{ description }}</h3>
    <p class="condition">Condition: {{ condition }}</p>
    <button @click="addItemToCart()" class="buy">Add to Cart</button>
  </div>
</template>

<script>
import CartView from "../views/CartView.vue";
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

  methods: {
    addItemToCart() {
      this.items.push([cart]);
    },
  },
};
</script>

<style></style>
