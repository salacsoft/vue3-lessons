<template>
  <div>
    <div v-html="hack"></div>
    <div v-html="name"></div>
    <div v-text="channel"></div>
  </div>
</template>

<script>

  export default {
    name: 'App',
   data() {
     return {
       name: "<i>Joseph</i>",
       channel: "Youtube",
       hack: `<a href="#" onclick="alert('you have been hacked')"> win a prize </a>`
     }
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
