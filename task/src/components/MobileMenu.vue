<script lang="ts" setup>
    import { ref } from 'vue'
    import { LTR } from 'element-plus/es/components/virtual-list/src/defaults';
    const handleOpen = (key: string, keyPath: string[]) => {
        console.log(key, keyPath)
    }
    const handleClose = (key: string, keyPath: string[]) => {
        console.log(key, keyPath)
    }
    const drawer = ref(false)
  </script>
  

<template>
    <img src="/mobilemenu.png" @click="drawer = true" style="cursor:pointer;" />
    <el-drawer
      v-model="drawer"
      :with-header="false"
      :direction="LTR"
      size="70%"
    >
    <el-menu
        default-active="2"
        class="el-menu-vertical-demo"
        @open="handleOpen"
        @close="handleClose"
      >
        <el-sub-menu index="1">
          <template #title >
            <span class="first">View All Products</span>
          </template>
            <el-menu-item index="1-1" class="second">item one</el-menu-item>
            <el-menu-item index="1-2" class="second">item two</el-menu-item>
            <el-menu-item index="1-3" class="second">item three</el-menu-item>
          <el-sub-menu index="1-4">
            <template #title >
                <span class="second">item four</span>
            </template>
            <el-menu-item index="1-4-1" class="third">item one</el-menu-item>
          </el-sub-menu>
        </el-sub-menu>
        <el-menu-item index="2">
          <span class="first">Hot Products</span>
        </el-menu-item>
        <el-menu-item index="3">
          <span class="first">Brands</span>
        </el-menu-item>
        <el-menu-item index="4">
          <span class="first">About Us</span>
        </el-menu-item>
      </el-menu>
    </el-drawer>
</template>

<style scoped>
.first{
    font-weight: 700;
}
.second{
    font-weight: 500;
    color:#337ecc;
}
.third{
    font-weight: 500;
}
::v-deep .el-sub-menu__title:hover {
    color: #337ecc;
}
::v-deep .el-menu-item:hover {
    color: #337ecc;
}
</style>