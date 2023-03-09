
<script>
 import test from "../components/test.vue"
 </script>



<template>
  <div class="about">
    <h1>cool jit</h1>
    <button @click = count++">
    Count is {{ count }}</button>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
