<template>
<div>
<b-container>
    <support-card></support-card>
  </b-container>
</div>
</template>

<script>
// @ is an alias to /src
//import HelloWorld from "@/components/HelloWorld.vue";
//import HelloWorld from "@/components/HelloWorld.vue";
import SupportCard from "@/components/SupportCard.vue"

export default {
  name: "Home",
  components: {
    "support-card": SupportCard,
    },
};
</script>
