<template>
  <div>
    <button>{{props.title}}</button>
  </div>
</template>

<script setup>
const props = defineProps({
  title: {
    default: "Click me",
    type: String,
    required: false
  }
});
</script>

<style>
</style>