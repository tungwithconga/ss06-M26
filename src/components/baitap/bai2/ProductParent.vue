<template>
  <div>
    <h1>Dữ liệu trong component cha</h1>
    <ProductChildren :product="product" />
  </div>
</template>

<script setup>
import ProductChildren from './ProductChildren.vue'

const product = {
  id: 1,
  name: 'Bưởi Ba Roi',
  price: 12000,
  quantity: 10
}
</script>
