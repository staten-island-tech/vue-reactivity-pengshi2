    <script>
    import ShoppingCart from "../components/shoppingCart.vue";
     import { store } from "../components/store.js";
    import storeInventory from "../components/storeInventory.vue";
    export default {
    data() {
        return {
            store,
        };
    },
    components: { ShoppingCart }
};
    </script>
<template>
  <div class ="cartview">
    <h1>Here is your shopping cart so far!</h1>
   <div class="cart">{{ store.cart.name }}</div>
    <ShoppingCart v-for="item in store.cart" :key= "item.name" 
    :name="item.name" :image="item.image" :price="item.price"
      :description="item.description" :condition="item.condition" />
  </div>
</template>


<style>
/* font-family: "Delicious Handrawn", */
/* cursive; */
</style>
