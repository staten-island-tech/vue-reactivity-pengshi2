<template>
    <div class="coolcard">
    <h2 class="name"> NAME:{{ name }}</h2>
    <p class="price"> PRICE: {{ price }}</p>
    <h3 class="description">{{ description }}</h3>
    <p class="condition">Condition: {{ condition }}</p>

    <storeInventory
    v-for="item in store.cart"
    :name="item.name"
    :image="item.image"
    :price="item.price"
    :description="item.description"
    :condition="item.condition"
  />
  </div>

  </template>
  
  <script>
  import storeInventory from "./storeInventory.vue";
  import { store } from "../components/store.js"
    components: { storeInventory, store }
  export default {
     data() {
     return {
    store,
}
    },
    props: {
    name: String,
    price: Number,
    description: String,
    image: String,
    condition: String,
  },
  }
  </script>
  
  <style></style>
  