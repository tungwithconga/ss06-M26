<template>
  <div>
    <button @click="sendMessage">Send message</button>
  </div>
</template>

<script setup>
const emit = defineEmits(['messageSent'])

const sendMessage = () => {
  emit('messageSent', 'Welcome to Rikkei Education')
}
</script>

<style scoped>
button {
  padding: 8px 16px;
  border: 1px solid #000;
  background-color: #fff;
  cursor: pointer;
  font-size: 16px;
}
</style>
