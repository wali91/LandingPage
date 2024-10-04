<template>
  <NavBar/>
  <formtalk/>
  <Footer/>
</template>

<script>
import NavBar from './NavBar.vue';
import Footer from './Footer.vue';
import formtalk from './fortalk/formtalk.vue'


/* eslint-disable vue/multi-word-component-names */
export default {
  name: 'BlogPage',
  components:{
    NavBar,
    Footer,
    formtalk

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
