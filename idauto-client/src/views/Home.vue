<template>
<div>
<b-container>
  <b-row align-v="center">
    <home-dashboard></home-dashboard>
  </b-row>|      
  </b-container>
      <b-container>  
      <b-row id="main-box" class="text-center">
        <b-col><person-card></person-card></b-col>
        <b-col cols="8"><Todos v-bind:todos="todos" /></b-col>
        </b-row>
      </b-container> 
</div>
</template>

<script>
// @ is an alias to /src
import Todos from '@/components/Todos';
import PersonCard from '@/components/PersonCard.vue';
import  HomeDashboard from "@/components/HomeDashboard.vue"

export default {
  name: "Home",
  components: {
    "home-dashboard": HomeDashboard,
    "person-card": PersonCard,
    Todos
    },
    data() {
    return {
      todos: [
        {
          id: 1,
          title: "Benjamin Salazar",
          completed: false
        },
        {
          id: 2,
          title: "Howard Cole",
          completed: true
        }
      ]
    }
  }
    
};
</script>
