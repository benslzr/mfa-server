<template>
  <div id="app">
    <b-container fulid>
      <div id="nav">
        <top-header></top-header>
      </div>
        <router-view/>
        <my-footer></my-footer>
      </b-container>
    </div>
</template>
<script>
import TopHeader from "@/components/TopHeader.vue";
import Footer from './components/Footer.vue';

// @ is an alias to /src
export default {
  name: 'app',
  components: {
    "top-header": TopHeader,
    "my-footer": Footer
  },
};
</script>
<style lang="scss">
.main-content {
  min-height: 350px;
}

#main-box {
  background: white;
  color: black;
  border-radius: 5px;
  min-height: 250px;
  border-style: solid;
  border-width: thin;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #e5e4e4;
  background: rgb(2,0,36);
  background: radial-gradient(circle, rgba(255,255,255,1) 33%, rgba(229,228,228,1) 72%);
}

#nav {
  padding: 30px;
  a {
    &.router-link-exact-active {
      color: #e32626;
    }
  }
}
</style>
