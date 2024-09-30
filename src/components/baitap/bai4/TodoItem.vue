<template>
  <div>
    <h2>-------- TodoItem Component --------</h2>
    <button @click="deleteItem">Delete</button>
  </div>
</template>

<script setup>
const emit = defineEmits(['deleteItem'])

const deleteItem = () => {
  const id = 1;
  emit('deleteItem', id)
}
</script>
