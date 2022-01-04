<template>
  <el-col :span="5">
    <el-menu
        default-active="4"
        class="el-menu-vertical-demo"
        style="width: 200px;min-height: 100vh"
    >
      <el-submenu index="1" >
        <template>
          <span>导航一</span>
          <i class="el-icon-location"></i>
        </template>
        <el-menu-item index="1-1">选项1</el-menu-item>
        <el-menu-item index="1-2">选项1</el-menu-item>
      </el-submenu>
      <el-menu-item index="2">
        <i class="el-icon-menu"></i>
        <span slot="title">导航二</span>
      </el-menu-item>
      <el-menu-item index="3">
        <i class="el-icon-document"></i>
        <span slot="title">导航三</span>
      </el-menu-item>
      <el-menu-item index="4">
        <i class="el-icon-setting"></i>
        <span slot="title">导航四</span>
      </el-menu-item>
    </el-menu>
  </el-col>
</template>

<script>
export default {
  name: "Aside"
}

</script>

<style scoped>

</style>