@@ -0,0 +1,85 @@
<script>
export default {
  data() {
    return {
      list: [
        { id: 1, name: "Gateron Red", price: 0.35 },
        { id: 2, name: "Kaihl Box Creams", price: 1.5 },
        { id: 3, name: "Kaihl Box Jades", price: 0.4 },
        { id: 4, name: "Zealios V2", price: 1.1 },
        { id: 5, name: "Gateron Yellows", price: 0.2 },
        { id: 6, name: "Gateron Ink Black V2", price: 0.85 },
        { id: 7, name: "Drop Holy Panda X", price: 1 },
        { id: 8, name: "Kaihl Box Royal", price: 0.2 },
        { id: 9, name: "Novelkeys X Kaihl Sherbert", price: 0.45 },
        { id: 10, name: "Roselios Silent", price: 1.3 },
      ],
    };
  },
};
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "./components/HelloWorld.vue";
import storeInventory from "./components/storeInventory.vue";
</script>

<template>
  <li v-for="(item, price) in list" :key="price">{{ name }}</li>
  <header>
    <img
      alt="Vue logo"
      class="logo"
      src="@/assets/logo.svg"
      width="125"
      height="125"
    />

    <div class="wrapper">
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
