<template>
  <el-header style="background-color: #409EFF;color: white">
    <el-row>
      <el-col :span="22">
        <div class="grid-content bg-purple">
          <p>个人信息系统</p>

        </div>
      </el-col>
      <el-col :span="2">
        <div class="grid-content bg-purple-light" style="margin-top: 15px">
          <i class="el-icon-user"></i>
          <el-dropdown>
            <span class="el-dropdown-link" style="color: white">用户</span>
            <template #dropdown>
              <el-dropdown-menu>
                <el-dropdown-item>个人信息</el-dropdown-item>
                <el-dropdown-item>修改密码</el-dropdown-item>
                <el-dropdown-item>退出系统</el-dropdown-item>
              </el-dropdown-menu>
            </template>
          </el-dropdown>

        </div>
      </el-col>
    </el-row>
  </el-header>
</template>

<script>

</script>

<style scoped>

</style>