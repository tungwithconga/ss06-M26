<template>
  <div>
    <MessageChildren @messageSent="handleMessage" />
    <div v-if="message" class="notification">
      <p>{{ location }} says</p>
      <p>{{ message }}</p>
      <button @click="clearMessage">OK</button>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import MessageChildren from './MessageChildren.vue'

const message = ref('')
const location = ref('')

const handleMessage = (msg) => {
  message.value = msg
  location.value = window.location.host
}

const clearMessage = () => {
  message.value = ''
}
</script>

<style scoped>
.notification {
  background-color: #333;
  color: #fff;
  padding: 16px;
  border-radius: 8px;
  width: 300px;
  position: relative;
}

button {
  padding: 8px 16px;
  background-color: #00f;
  color: #fff;
  border: none;
  cursor: pointer;
  border-radius: 8px;
  font-size: 16px;
}

button:hover {
  background-color: #007bff;
}
</style>
