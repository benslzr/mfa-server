<template>
  <div id="app">
    <div id="nav">
      <b-container><top-header></top-header></b-container>
      <div id="lower-nav">
      <b-container>
        <lower-header></lower-header>
        <Todos v-bind:todos="todos" />
        </b-container>
    </div>
    </div>
    <div>
      <b-container>
        <router-view/>
      </b-container>
    </div>
  </div>
</template>
<script>
import Todos from './components/Todos';
import TopHeader from "@/components/TopHeader.vue"
import  LowerHeader from "@/components/LowerHeader.vue"
// @ is an alias to /src
export default {
  name: 'app',
  components: {
    "top-header": TopHeader,
    "lower-header": LowerHeader,
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
<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background: rgb(2,0,36);
  background: radial-gradient(circle, rgba(2,0,36,0.02238581730769229) 0%, rgba(255,193,200,1) 56%);
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
