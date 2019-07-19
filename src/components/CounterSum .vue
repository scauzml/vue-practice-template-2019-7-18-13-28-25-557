<template>
  <div class="hello">
    <div>
     和{{sum1}}
    </div>
  </div>
</template>

<script>
export default {
  name: "CounterSum",
  props:{
      sum1:Number
  },
  data() {
    return {
     
    };
  },
  
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
