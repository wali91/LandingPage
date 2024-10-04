<template>
  <NavBar />
  <Questions />
  <Footer />
</template>

<script>
import Footer from './Footer.vue';
import Questions from './forfaq/Questions.vue';
import NavBar from './NavBar.vue';




export default {
  name: 'FAQ',
  components:{
    NavBar,
    Questions,
    Footer

  },
  props: {
   content: String
  },
  created() {
    this.language=localStorage.getItem('language')
  },
  methods:{
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

  
};
</script>

<style scoped>

</style>
