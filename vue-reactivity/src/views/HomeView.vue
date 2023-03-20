<script>
export default {
  name: "HomeView",
  components: {},
  data() {
    return {
      items: items,
    };
  },
};
</script>

<template>
  <li v-for="item in list">
    {{ item.name }}
  </li>
</template>
