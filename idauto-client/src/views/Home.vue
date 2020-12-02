<template>
<div>
<b-container>
  <b-row align-v="center">
    <home-dashboard></home-dashboard>
    <person-card></person-card>
  </b-row>
  </b-container>
</div>
</template>

<script>
// @ is an alias to /src
//import HelloWorld from "@/components/HelloWorld.vue";
//import HelloWorld from "@/components/HelloWorld.vue";
import PersonCard from "@/components/PersonCard.vue"
import  HomeDashboard from "@/components/HomeDashboard.vue"

export default {
  name: "Home",
  components: {
    "person-card": PersonCard,
    "home-dashboard": HomeDashboard
    },
};
</script>
