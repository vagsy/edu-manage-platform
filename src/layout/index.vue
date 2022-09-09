<template>
  <el-container>
    <el-aside width="200px">
      <left-aside />
    </el-aside>
    <el-container>
      <el-header>
        <Header />
      </el-header>
      <el-main>
        <!-- 子路由出口 -->
        <router-view />
      </el-main>
    </el-container>
  </el-container>
</template>
<script lang="ts">
import Vue from 'vue'
import LeftAside from './components/left-aside.vue'
import Header from './components/header.vue'

export default Vue.extend({
  name: 'LayoutIndex',
  components: {
    LeftAside,
    Header
  }
})
</script>

<style lang="scss" scoped>
.el-container {
  min-height: 100vh;
  min-width: 980px;
}

.el-aside {
  background: #d3dce6;
}

.el-header {
  background: #fff;
}

.el-main {
  background: #e9eef3;
}
</style>
