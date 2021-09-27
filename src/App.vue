<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->
    <Header/>
    <router-view/>
    <Footer/>
  </div>
</template>
<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
// import HelloWorld from '../components/HelloWorld.vue'; 
import Footer from './components/Footer.vue'
import Header from './components/Header.vue'

@Component({
  components: {
    Footer,
    Header
  },
})
export default class Home extends Vue {}
</script>

<style lang="less">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
body {
  font-family: 'Roboto', sans-serif;
}
a {
  color: #000;
}
</style>
