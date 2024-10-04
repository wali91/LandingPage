<template>
  <NavBar/>
  <MCASH/>
  <World/>
  <Success/>
  <Footer/>
</template>

<script>
import NavBar from './NavBar.vue';
import Footer from './Footer.vue';
import MCASH from './forpartners/MCASH.vue';
import World from './forpartners/World.vue';
import Success from './forpartners/Success.vue';



/* eslint-disable vue/multi-word-component-names */
export default {
  name: 'PartnersPage',
  data() {
    return {
      content: {}
    }},
  components:{
    NavBar,
    Footer,
    MCASH,
    World,
    Success

  },methods:{
    scrolltotop() {
      window.scrollTo({
  top: 0,
  behavior: 'smooth'
});
    }
  },
  mounted() {
    console.log('partner')
    this.scrolltotop()
  }
}
/* eslint-enable vue/multi-word-component-names */
</script>

<style scoped>

</style>
