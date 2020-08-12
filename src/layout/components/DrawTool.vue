<template>
  <div class="drawTool">
    <el-menu default-active="1-4-1" class="el-menu-vertical-demo" :collapse="isCollapse" @open="handleOpen" @close="handleClose">
      <el-menu-item index="1">
        <i class="el-icon-location-outline" />
        <span slot="title">定位</span>
      </el-menu-item>
      <el-menu-item index="2">
        <i class="el-icon-menu" />
        <!-- <span slot="title">导航二</span> -->
      </el-menu-item>
      <el-menu-item index="3">
        <i class="el-icon-document" />
        <!-- <span slot="title">导航三</span> -->
      </el-menu-item>
      <el-menu-item index="4">
        <i class="el-icon-setting" />
        <!-- <span slot="title">导航四</span> -->
      </el-menu-item>
    </el-menu>
  </div>
</template>

<script>
export default {
  name: 'DrawTool',
  data() {
    return {
      isCollapse: true
    }
  },
  methods: {
    handleOpen(key, keyPath) {
      console.log(key, keyPath)
    },
    handleClose(key, keyPath) {
      console.log(key, keyPath)
    }
  }

}
</script>

<style lang="scss">
.drawTool {
  overflow: hidden;
  position: relative;
   .el-menu-vertical-demo:not(.el-menu--collapse) {
    width: 60px;
  }
}

</style>
