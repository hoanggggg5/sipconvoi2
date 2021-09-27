<template>
  <div class="home">
    <ProductList/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
// import HelloWorld from '../components/HelloWorld.vue'; 
import ProductList from '../components/ProductList.vue'
import Footer from '../components/Footer.vue'
import Header from '../components/Header.vue'

@Component({
  components: {
    // HelloWorld,
    ProductList,
    Footer,
    Header
  },
})
export default class Home extends Vue {}
</script>

