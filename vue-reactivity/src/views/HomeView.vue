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
          name: "Bayonet | Night",
          price: 450,
          condition: "Minimal Wear",
          description:
            "It has individual parts spray-painted solid colors in a night ops color scheme.",
          image:
            "https://steamcdn-a.akamaihd.net/apps/730/icons/econ/default_generated/weapon_bayonet_so_night_light_large.11b2117af2e0f240111305857ab93e0091e347ed.png",
        },
        {
          id: 2,
          name: "Butterfly Knife | Crimson Web",
          price: 1300,
          condition: "Field-Tested",
          description:
            "It has been painted using a spider web-patterned hydrographic over a red base coat and finished with a semi-gloss topcoat.",
          image:
            "https://steamcdn-a.akamaihd.net/apps/730/icons/econ/default_generated/weapon_knife_butterfly_hy_webs_light_large.8e3a3668a8678a4ce56b2675c60d7ec6a756827a.png",
        },
        {
          id: 3,
          name: "Huntsman Knife | Slaughter",
          price: 360,
          condition: "Minimal Wear",
          description:
            "It has been painted in a zebra-stripe pattern with aluminum and chrome paints with various reflectivities, and has then been covered with a tomato red candy coat.",
          image:
            "https://steamcdn-a.akamaihd.net/apps/730/icons/econ/default_generated/weapon_knife_tactical_am_zebra_light_large.1296d76d34f1e5738524c808f365584a38aaf6bf.png",
        },
        {
          id: 4,
          name: "Skeleton Knife | Case Hardened",
          price: 1450,
          condition: "Factory New",
          description:
            " It has been color case-hardened through the application of wood charcoal at high temperatures.",
          image:
            "https://steamcdn-a.akamaihd.net/apps/730/icons/econ/default_generated/weapon_knife_skeleton_aq_oiled_light_large.822bad0bf51e44a83631245c24ca5c2999df0948.png",
        },
        {
          id: 5,
          name: "M9 Bayonet | Doppler",
          price: 1232,
          condition: "Factory New",
          description:
            "It has been painted with black and silver metallic paints using a marbleizing medium, then candy coated.",
          image:
            "https://steamcdn-a.akamaihd.net/apps/730/icons/econ/default_generated/weapon_knife_m9_bayonet_am_doppler_phase1_light_large.1a9960a6bba1a82aeab00b0207b4ff7c423a1f06.png",
        },

        {
          id: 6,
          name: "Gut Knife | Rust Coat",
          price: 154,
          condition: "Well-Worn",
          description:
            "It is still perfectly operational although the exterior surfaces have rusted.",
          image:
            "https://steamcdn-a.akamaihd.net/apps/730/icons/econ/default_generated/weapon_knife_gut_aq_steel_knife_light_large.d56ab6033e5da6115f6af2aba93bae8edde57cb3.png",
        },
        {
          id: 7,
          name: "Flip Knife | Fade",
          price: 1150,
          condition: "Factory New",
          description:
            " It has been painted by airbrushing transparent paints that fade together over a chrome base coat.",
          image:
            "https://steamcdn-a.akamaihd.net/apps/730/icons/econ/default_generated/weapon_knife_flip_aa_fade_light_large.811f8e8af2e00675c047a9c1e9f04bbe5ace83b1.png",
        },
        {
          id: 8,
          name: "Bowie Knife | Marble Fade",
          price: 447,
          condition: "Factory New",
          description:
            "It has been painted with black and silver metallic paints using a marbleizing medium, then candy coated in three colors.",
          image:
            "https://steamcdn-a.akamaihd.net/apps/730/icons/econ/default_generated/weapon_knife_survival_bowie_am_marble_fade_light_large.ee64f39331b11b42f6ef7e00f570bc0da09cf0ee.png",
        },
        {
          id: 9,
          name: "Talon Knife | Ultraviolet",
          price: 700,
          condition: "Factory New",
          description:
            "It has individual parts spray-painted solid colors in a black and purple color scheme.",
          image:
            "https://steamcdn-a.akamaihd.net/apps/730/icons/econ/default_generated/weapon_knife_widowmaker_so_purple_light_large.8338e07caf8f6c129754b605709612b5e3d1679d.png",
        },
        {
          id: 10,
          name: "Karambit | Gamma Doppler",
          price: 1700,
          condition: "Factory New",
          description:
            "It has been painted with black and silver metallic paints using a marbleizing medium, then candy coated.",
          image:
            "https://steamcdn-a.akamaihd.net/apps/730/icons/econ/default_generated/weapon_knife_karambit_am_gamma_doppler_phase1_light_large.769cf2ab676ea2a7d7322c258f57bac8dca00336.png",
        },

        {
          id: 11,
          name: "Stiletto Knife | Tiger Tooth",
          price: 670,
          condition: "Factory New",
          description:
            "It has been anodized orange and hand-etched in a tiger stripe pattern.",
          image:
            "https://steamcdn-a.akamaihd.net/apps/730/icons/econ/default_generated/weapon_knife_stiletto_an_tiger_orange_light_large.dd59dfda5a30c3e7b0dbe256831ec91c4405bc34.png",
        },

        {
          id: 12,
          name: "Falchion Knife | Autotronic",
          price: 300,
          condition: "Minimal Wear",
          description:
            "It has been anodized red and uses steel mesh to lighten the weight.",
          image:
            "https://steamcdn-a.akamaihd.net/apps/730/icons/econ/default_generated/weapon_knife_falchion_gs_falchion_autotronic_light_large.6bd228d144c25d432c94cd77a5c41ecb8a31b8fb.png",
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
    :image="item.image"
    :price="item.price"
    :description="item.description"
    :condition="item.condition"
  />
</template>

<style>
.coolcard {
  background-color: aliceblue;
  text-align: center;
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  justify-content: center;
  margin: 20px auto;
  border: 1px solid black;
  padding: 10px;
  scale: 80%;
  font-family: "Delicious Handrawn", cursive;
}

body,
html {
  margin: 0;
  padding: 0;
}

.buy {
  margin-top: 10px;
  left: 60px;
  max-height: 15px;
}

.remove {
  margin-top: 10px;
  left: 60px;
  max-height: 15px;
}
</style>
