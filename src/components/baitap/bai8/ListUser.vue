<template>
  <div>
    <h2>-------- List User --------</h2>
    <button @click="showForm = true">Add user</button>
    <FormAddUser v-if="showForm" @closeForm="closeForm" />
  </div>
</template>

<script setup>
import { ref } from 'vue'
import FormAddUser from './FormAddUser.vue'

const showForm = ref(false)

const closeForm = () => {
  showForm.value = false
}
</script>

<style scoped>
button {
  padding: 10px 20px;
  background-color: #007bff;
  color: white;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  font-size: 16px;
}
</style>
