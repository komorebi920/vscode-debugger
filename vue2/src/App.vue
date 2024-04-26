<template>
  <div id="app">
    <div>{{ num }}</div>
    <Button @change="onChange" />
  </div>
</template>

<script>
import Button from "./components/Button.vue";

export default {
  name: "App",
  components: {
    Button
  },
  data() {
    return {
      num: 0
    };
  },
  methods: {
    onChange() {
      this.num++;
    }
  }
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
</style>
