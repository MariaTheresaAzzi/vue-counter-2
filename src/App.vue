<script>
export default {
  data() {
    return {
      count: 0,
    };
  },
  methods:{
    addToCount(){
      this.count = this.count + 1;
    },
    substractToCount(){
      this.count = this.count - 1;
    }
  }
};
</script>

<template>
  <div class="all">
    <h4>The current count ...</h4>
    <h1>
      {{ count }}
    </h1>
    <div>
      <button @click="substractToCount()">-</button>
      <button @click="addToCount()">+</button>
    </div>
  </div>
</template>

<style scoped>
.all {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
</style>
