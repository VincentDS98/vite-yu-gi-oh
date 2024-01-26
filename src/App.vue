<script >
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import axios from 'axios';



export default {
  data() {
    return { 
        baseUrl: 'https://db.ygoprodeck.com/api/v7/cardinfo.php?num=20&offset=0',
        card: []
    };

  },
  components: {
    AppHeader,
    AppMain,
    AppFooter 

  },
  methods:{

  },
  mounted() {
    axios.get(this.baseUrl).then((response) => {
      //console.log(response.data)
      this.card = response.data;
      console.log(this.card); 
    });
  }
  
}
</script>

<template>

   

    <AppHeader/>

    <AppMain/>

    <AppFooter/>
</template>

<style lang="scss" >
@use "assets/scss/main" as *;
@import "assets/scss/partials/reset";
// Import all of Bootstrap's CSS
//@import "~bootstrap/scss/bootstrap";


</style>
