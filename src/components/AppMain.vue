<script >

export default {
  data() {
    return { 
      
    };
  },
  props: {
    allCards: Array
  }
  
}
</script>

<template>
   <main>
      <div class="container">
        <div class="row">
          <div class="col" v-for="(cards, i) in allCards" :key="i">
            Carte
          </div>
        </div>
      </div>
   </main>
</template>

<style scoped>

</style>
