<template>
  <div>
    <Modal title="Thông báo từ hệ thống" @close="handleModalClose">
      Đây là nội dung của modal. Bạn có thể đóng modal bằng cách nhấn vào nút 'Close'.
    </Modal>
  </div>
</template>

<script setup>
const handleModalClose = () => {
  console.log('Modal has been closed.')
}
</script>
