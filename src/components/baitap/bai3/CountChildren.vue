<template>
  <div>
    <h2>-------- Children Component --------</h2>
    <button @click="increment">Increment</button>
  </div>
</template>

<script setup>
const emit = defineEmits(['increment'])

const increment = () => {
  emit('increment')
}
</script>
