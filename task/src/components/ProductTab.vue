<script lang="ts" setup>
  import type { TabsPaneContext } from 'element-plus'
  import ProductCarousel from "./ProductCarousel.vue"  
  const handleClick = (tab: TabsPaneContext, event: Event) => {
    console.log(tab, event)
  }
  </script>

<template>
    <el-row justify="space-around">
        <el-col :span="22">
            <el-tabs
            model-value="second"
            type="border-card"
            class="demo-tabs"
            @tab-click="handleClick"
            >
            <el-tab-pane label="Why Idirectpromo"  name="first">
              <span>
                Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum
              </span>
            </el-tab-pane>
            <el-tab-pane label="Latest Products" name="second">
              <ProductCarousel/>
            </el-tab-pane>
          <el-tab-pane label="Best Seller" name="third">
              <ProductCarousel/>
          </el-tab-pane>
        </el-tabs>
      </el-col>
    </el-row>
</template>

  <style scoped>
.el-tabs--border-card>.el-tabs__header {
    margin-bottom: 0px;
}
.el-tabs--border-card>.el-tabs__content {
    height: 400px;
    border: 1px solid #eeeeee;
    border-radius: 30px;
    box-shadow: 0px 3px 9px 0px rgb(0 0 0 / 9%);
  }
</style>

<style>
.el-tabs--border-card>.el-tabs__header{
  height: 40px;
  background-color: white;
  border: 0;
}
.el-tabs--border-card>.el-tabs__header .el-tabs__item.is-top{
  width: max(150px,calc(100vw * 250 / 1920));
  border: 1px var(--el-border-color) solid;
}
.el-tabs--border-card>.el-tabs__header .el-tabs__item.is-active {
  color: white;
  background-color: red;
}
.el-tabs--border-card>.el-tabs__header .el-tabs__item.is-top:hover{
  color:grey;
}
.el-tabs--border-card>.el-tabs__header .el-tabs__item.is-active:hover{
  color: white;
}
</style>