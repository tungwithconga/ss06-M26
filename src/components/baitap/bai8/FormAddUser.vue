<template>
  <div class="form-overlay">
    <div class="form-container">
      <h3>Form Add User</h3>
      <form>
        <label for="name">Name</label>
        <input type="text" id="name" />

        <label for="email">Email</label>
        <input type="email" id="email" />

        <label for="address">Address</label>
        <input type="text" id="address" />

        <button type="button" @click="closeForm" class="close-btn">Close</button>
      </form>
    </div>
  </div>
</template>

<script setup>
const emit = defineEmits(['closeForm'])

const closeForm = () => {
  emit('closeForm')
}
</script>

<style scoped>
.form-overlay {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: rgba(0, 0, 0, 0.5);
  display: flex;
  justify-content: center;
  align-items: center;
}

.form-container {
  background-color: white;
  padding: 20px;
  border-radius: 8px;
  width: 300px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

form {
  display: flex;
  flex-direction: column;
}

input {
  margin-bottom: 10px;
  padding: 8px;
  border: 1px solid #ddd;
  border-radius: 4px;
}

.close-btn {
  background-color: red;
  color: white;
  padding: 8px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  font-size: 14px;
}
</style>
