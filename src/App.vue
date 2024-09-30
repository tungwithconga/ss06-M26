<template>
<div>
  <h1>homepage</h1>
  <ParentComponent/>

  <BaseButton title="Click Me" />
  <BaseButton title="Add product" />
  <SlotComponent>
    <!-- Nội dung này sẽ chích là slot thông qua thẻ slot  -->
    <a href="">FaceBook</a>
  </SlotComponent>
</div>

</template>

<script setup>
import ParentComponent from "./components/ParentComponent.vue"
import BaseButton from "./components/BaseButton.vue"
import SlotComponent from "./components/SlotComponent.vue"

import ParentComponent from "./components/baitap/bai1/ParentComponent.vue"
</script>

<style>

</style>