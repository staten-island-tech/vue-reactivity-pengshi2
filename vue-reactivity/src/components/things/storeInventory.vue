<template>
  <div class="Coolcard">
    <h2>{{ item.name }}</h2>
    <h3 class="cost">${{ item.price }}</h3>
    <p class="Description">Description: {{ Description }}</p>
  </div>
</template>

<script>
export default {
  props: ["item"],
  computed: {
    Description() {
      return this.item.Description.substring(0, 150);
    },
  },
};
</script>

<style></style>
