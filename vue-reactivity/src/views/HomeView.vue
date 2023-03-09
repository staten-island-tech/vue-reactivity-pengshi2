<script>
import test from "../components/test.vue";

export default {
  components: {},
  data() {
    return {
      name: "Joe",
      smart: true,
    };
  },
};
</script>

<template>
  <h1 v-if="smart">{{ name }}</h1>
  <h1 v-else>They are not smart</h1>
  <h2>{{ message }}</h2>
  <main>
    <test />
  </main>
</template>
