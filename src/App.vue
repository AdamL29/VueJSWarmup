<template>
  <div id="app">
    <FunComponent/>
    <!-- <Secrets/> NOT NEEDED-->
  </div>
</template>

<script>
import FunComponent from '@/components/FunComponent.vue';
// import Secrets from '@/components/Secrets.vue'; NOT NEEDED

export default {
  name: 'App',
  components: {
    FunComponent,
    // Secrets, NOT NEEDED
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
