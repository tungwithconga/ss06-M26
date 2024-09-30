<template>
<div>
    <h1>Parent Component</h1>
    <p>--------------------------------------------</p>
   <!-- Sử dụng Component con -->
   <!-- Bước 2 trong component cha gọi props được khai báo bên con và truyền giá trị cho nó -->
   <ChildrenComponent :userNameProps="userName" :ageProps="age" :userInfoProps="userInfo"/> 
</div>

</template>

<script setup>
import ChildrenComponent from './ChildrenComponent.vue'
const userName = "Nguyen Van A";
//Tạo biến tuổi và truyền từ ParentComponent xuống ChildrenComponent
const age = 20;
const userInfo = {
    id:1,
    name:"Nguyễn Văn B",
    age:21
};
</script>

<style>

</style>