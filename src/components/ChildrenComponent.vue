<template>
<div>
  <h1>Children Component</h1>
  <!-- Bước 3 :Lấy giá trị từ props và render dữ liệu -->
  <h3>UserName of ChildrenComponents: {{ userNameProps }}</h3>
  <h3>Age of ChildrenComponents: {{ ageProps }}</h3>
  <h3>userInfoProps of ChildrenComponents: {{ userInfoProps }}</h3>
  <p>----------------------------------------</p>
</div>

</template>

<script setup>
//Bước 1 :Định nghĩa props bên trong component con
 const {userNameProps,ageProps,userInfoProps} = defineProps(
 ["userNameProps",
 "ageProps",
 "userInfoProps"]);
 console.log("userinfoProps: " , userInfoProps)
</script>

<style>
</style>