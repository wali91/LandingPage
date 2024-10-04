<template>
<div class="container-fluid">
  <div class="container">
    <div class="row justify-content-center">
      <div class="col-6">
        <h2 class="title"> {{$t('partner_page.World.Join')}} </h2>
        <p>
          {{ $t('partner_page.World.Paragraph') }}
        </p>
        <div class="buttons pt-4">
          <a class="btn" href="https://dev.wabiz.id/register/9459e36b873845d484cee7b87bc5e4ca:cc0b5b800dc9c50eebe855dac455ead631e582e630793f55cfb6e17f0ab00e5e3bcc0a61b6a0fe7777b4bf38f0c0ad4aee83ef3dd4e1e59bf154c19d72700cda0f76da5d69dae7d7e0be6d442fe08c700117bca0a86c877845982d91913c4d30"  role="button">{{ $t('partner_page.World.Register') }}</a>
          <a class="btn ms-3" @click="toFormpage" role="button">{{ $t('partner_page.World.Talk') }}</a>
        </div>
      </div>
      
      <div class="col-6  worldmap">
        <img src="@/assets/public/worldmap.svg" height="330">
      </div>

      <div class="w-100 my-5"></div>

      <div class="col-6 mt-2">
        <img src="@/assets/public/locations.svg" height="300">

      </div>
      <div class="col-6">
        <h2 class="title">Our Partners</h2>
        <div class="row">
          <div class="col-4">

          </div>
          <div class="col-4">
            
          </div>
          <div class="col-4">
            
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
</template>

<script>
export default {
 /* eslint-disable vue/multi-word-component-names */
  name: 'World',
  props: {
   content: String
  },
  data() {
    return {
      language: ''
    }
  },
  methods: {
    toFormpage() {
      this.$router.push(`/formspage`);
    }
  },
  created() {
    this.language=localStorage.getItem('language')
  }
  
};
</script>

<style scoped>
.container-fluid {
  width:100%;
  background-color:#009C77;
  font-family: metrophobic;
  color:white;
  padding-bottom: 5vh;
}
.title {
  font-weight: 600;
  margin-top:50px;
}
.container-fluid {
  padding-top: 8vh;
}
.btn {
  background-color:white;
  color:#009C77;
  width: 28%;
  border-radius: 60px;
}
</style>
