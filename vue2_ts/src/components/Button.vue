<template>
  <button type="button" @click="onClick">+1</button>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component
export default class Button extends Vue {
  onClick() {
    debugger;
    this.$emit("change");
  }
}
</script>
