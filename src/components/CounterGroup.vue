<template>
  <div class="counterGroub" >
    <input type="text" v-model.number="counterNum" >
    <div v-for="dd in counterNum" :key="dd" >
       <Count @putNum="toSum" @putNumtoDown="toDown"></Count>
    </div>   
    <CounterSum v-bind:sum1="sum"></CounterSum>
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
              counterNum:0,
              sum:0
      }
  },
  methods: {
    // enter () {
    //   this.$emit("sendcouter", this.counterNum) 

    // }
    toSum(){
      this.sum+=1
    },
    toDown(){
        this.sum-=1;
    }
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
