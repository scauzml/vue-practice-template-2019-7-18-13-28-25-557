<template>
  <div class="counterGroub">
    <input type="text" v-model.number="counterNum" >
    <button @click="build">点击</button>
    <div v-for="dd in counterNum" :key="dd" >
       <Count></Count>
    </div>
  </div>
</template>

<script>
import Count from './count'
export default {
  name: 'countgroub',
  components:{
    Count
  },
  data(){
      return {
              counterNum:0
      }
  },
  methods: {
    // enter () {
    //   this.$emit("sendcouter", this.counterNum) 

    // }
    build(){

    }
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
