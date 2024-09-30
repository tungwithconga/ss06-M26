<template>
  <div>
    <Card>
      <template #header>
        Thông tin sản phẩm
      </template>
      <template #body>
        Đây là mô tả ngắn gọn về sản phẩm này. Sản phẩm có các tính năng nổi bật và giá cả hợp lý.
      </template>
      <template #footer>
        <button @click="handleDetail" class="btn">Xem chi tiết</button>
      </template>
    </Card>
  </div>
</template>

<script setup>
const handleDetail = () => {
  console.log('Xem chi tiết sản phẩm')
}
</script>

<style scoped>
.btn {
  background-color: #007bff;
  color: white;
  border: none;
  padding: 8px 16px;
  border-radius: 4px;
  cursor: pointer;
}
.btn:hover {
  background-color: #0056b3;
}
</style>
