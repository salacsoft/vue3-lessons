<template>
  <div>
    <h1>{{name}}</h1>
    <div v-text="channel"></div>
    <h2 v-bind:id="headingId">Heads</h2>
    <h2 className="underline">Underline</h2>
    <h2 class="underline" v-bind:class="txtColor">Color</h2>
    <h3 v-bind:Class="isPromoted && 'promoted' ">Promoted Movie</h3>
  </div>
</template>

<script>

  export default {
    name: 'App',
   data() {
     return {
       name: "Joseph",
       channel: "Youtube",
       headingId: "heading",
       txtColor: "green",
       isPromoted: true
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
  .underline {
    text-decoration: underline;
  }

  .green {
    color: green;
  }

  .promoted {
    font-style: italic;
  }
</style>
