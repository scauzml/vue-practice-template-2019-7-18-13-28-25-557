<template>
  <div class="hello">
    <div>
     和{{sum}}
    </div>
  </div>
</template>

<script>
export default {
  name: "CounterSum",

  data() {
    return {
     
    };
  },
  computed:{
    sum(){
      return this.$store.getters.getSum;
    }
  }
  
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
