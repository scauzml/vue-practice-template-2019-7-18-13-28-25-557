<template>
  <div class="counterGroub" >
    <input type="text" v-model.number="counterNum" >
    <div v-for="dd in counterNum" :key="dd" >
       <Count></Count>
    </div>   
    <CounterSum></CounterSum>
  </div>

</template>

<script>
import Count from './count'
import CounterSum from './CounterSum '

export default {
  name: 'countgroub',
  components:{
    Count,
    CounterSum
  },
  data(){
      return {
         counterNum:0  
      }
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
