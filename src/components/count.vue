<template>
  <div class="hello">
    <div>
      <button @click="increase">+</button>
      <input type="text" v-model="a" />
      <button @click="descease">-</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "count",

  data() {
    return {
      a: 0,
    };
  },
  methods: {
    increase() {
      this.a++;
      
    },
    descease() {
      this.a--;
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
