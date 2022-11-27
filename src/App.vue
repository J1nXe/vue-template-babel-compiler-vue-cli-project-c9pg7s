<template>
  <h1>{{ title }}</h1>
  <input type="text" ref="name">
  <button @click="handelClick">Click ME</button>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      title: 'my fist Vau app:',
    };
  },
  methods: {
    handleClick() {
      console.log(this.$refs.name)
    },
  },
};
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
h1 {
  border-bottom: 10px;
}
</style>
