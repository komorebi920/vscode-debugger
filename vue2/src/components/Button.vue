<template>
  <button type="button" @click="onClick">+1</button>
</template>

<script>
export default {
  name: "Button",
  methods: {
    onClick() {
      this.$emit("change");
    }
  }
};
</script>
