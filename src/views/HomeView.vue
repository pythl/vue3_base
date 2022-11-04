<script setup lang="ts">
let obj = reactive({
  a: 1,
  b: 2,
  arr: ["11", "22"],
});
let handleChange = () => {
  obj.a = 3;
  console.log(obj);
};
</script>

<template>
  <main>
    <el-button @click="handleChange" type="success">Success</el-button>
    <el-button>Default</el-button>
    <el-button type="primary">Primary</el-button>
    <el-button type="success">Success</el-button>
    <el-button type="info">Info</el-button>
    <el-button type="warning">Warning</el-button>
    <el-button type="danger">Danger</el-button>
  </main>
</template>
