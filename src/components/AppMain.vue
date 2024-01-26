<script >

export default {
  data() {
    return { 
      
    };
  },
  
}
</script>

<template>
   <main>
      <div class="container">
        <div class="row">
          <div class="col" v-for="i in 20" :key="i">
            Personaggio
          </div>
        </div>
      </div>
   </main>
</template>

<style scoped>

</style>
