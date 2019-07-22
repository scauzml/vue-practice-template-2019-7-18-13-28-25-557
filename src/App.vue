<template>
  <div id="app">
    <CounterGroug ></CounterGroug>
  </div>
</template>

<script>

import CounterGroug from './components/CounterGroup'
export default {
  name: 'app',
  components: {
    CounterGroug
    
  },
  data(){
      return {
       
      }
  },
  methods:{
   
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
