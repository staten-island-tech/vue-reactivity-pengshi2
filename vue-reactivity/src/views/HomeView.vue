<script>
import storeInventory from "../components/storeInventory.vue";
export default {
  name: "HomeView",
  components: { storeInventory },
  data() {
    return {
      items: [
        {
          id: 1,
          name: "Gateron Red",
          type: "Linear",
          price: 0.35,
          description:
            "Gateron red is the most commonly used Gateron switch because it is a linear switch, making the typing sound quieter. The pressure is more moderate, light, and prolonged periods of typing will not feel tired. They are suitable for a variety of scenarios and also suitable for most people to use.",
          image: "",
        },
        {
          id: 2,
          name: "Kaihl Box Creams",
          price: 1.5,
          type: "Linear",
          description:
            "Known for their ultra-smooth travel, Cream switches are a top choice among linear fans in search of a truly seamless typing experience.",
          image: "",
        },
        {
          id: 3,
          name: "Kaihl Box Jades",
          price: 0.4,
          type: "Clicky",
          description:
            "Known for being extremely clicky and tactile, these switches are very loud and satisfying, great for typing but not so much gaming.",
          image: "",
        },
        {
          id: 4,
          name: "Zealios V2",
          price: 1.1,
          type: "Tactile",
          description:
            "Known as one of the most tactile switches the market has to offer, Zealios V2 are rather expensive however.",
          image: "",
        },
        {
          id: 5,
          name: "Gateron Yellows",
          price: 0.2,
          type: "Linear",
          description:
            "Linear switches for people looking for quality switches while on a tight budget. Well renowed for their exceptional performance for price.",
          image: "",
        },

        {
          id: 6,
          name: "Gateron Ink Black V2",
          price: 0.85,
          type: "Linear",
          description:
            "Gateron Black Ink V2's are from Gateron's premium line of switches. They feature a unique housing material and coated spring.  These switches are highly regarded within the community, and arguably one of the smoothest linears. ",
          image: "",
        },
        {
          id: 7,
          name: "Drop Holy Panda X",
          price: 1,
          type: "Tactile",
          description:
            "The Holy Panda experience has evolved. Introducing the Holy Panda X: the next iteration of tactile typing, optimized for an authentic feel with unrivaled consistency",
          image: "",
        },
        {
          id: 8,
          name: "Kaihl Box Royal",
          price: 0.2,
          type: "Tactile",
          description:
            "These switches are extremely tactile, almost as much as Zealios V2 while being a fraction of the cost, great for people who want to try out tactile switches.",
          image: "",
        },
        {
          id: 9,
          name: "Cherry MX Brown",
          price: 0.45,
          type: "Tactile",
          description:
            "The characteristic of this tactile switch is characterized by a noticeable feedback. The noiseless guidance of the CHERRY MX Brown trains the sure instinct and helps to act tactically and strategically.",
          image: "",
        },
        {
          id: 10,
          name: "Roselios Silent",
          price: 1.3,
          type: "Linear",
          description:
            "Roselio silents are known for their striking pink stems, and also being the quietest linear switches on the market, perfect for a work enviorment while still being smooth. ",
          image: "",
        },
      ],
    };
  },
};
</script>

<template>
  <storeInventory
    v-for="item in items"
    :name="item.name"
    :price="item.price"
    :image="item.image"
    :description="item.description"
    :type="item.type"
  />
</template>

<style>
.coolcard {
  text-align: center;
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  justify-content: center;
  scale: 80%;
}
</style>
