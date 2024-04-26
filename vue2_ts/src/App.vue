<template>
  <div id="app">
    <div>{{ num }}</div>
    <Button @change="onChange" />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import Button from "./components/Button.vue";

@Component({ components: { Button } })
export default class App extends Vue {
  num: number = 0;

  onChange() {
    this.num++;
  }
}
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
