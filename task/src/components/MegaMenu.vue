<script setup lang="ts">
import { ref } from 'vue'
import { ArrowDown } from '@element-plus/icons-vue'
import MobileMenu from './MobileMenu.vue';

const handleClick = () => {
  // eslint-disable-next-line no-alert
  alert('button click')
}
const activeIndex = ref('1')
const handleSelect = (key: string, keyPath: string[]) => {
  console.log(key, keyPath)
}
</script>

<template>
    <el-row justify="center" align="middle">
        <el-col :xs="10" :sm="10" :lg="0">
            <MobileMenu/>
        </el-col>
        <el-col :xs="4" :sm="10" :lg="0"> </el-col>
        <el-col :xs="0" :sm="0" :lg="20">
            <el-menu
                :default-active="activeIndex"
                class="el-menu-demo"
                mode="horizontal"
                @select="handleSelect"
                ellipsis="false"
                style="border:none; margin-top:10px; "
            >
                <el-menu-item index="1" style="border:none; height: auto;">
                    <el-dropdown>
                        <el-button type="primary">
                            <el-icon class="el-icon--left"><Menu /></el-icon>
                            View All Products
                            <el-icon class="el-icon--right"><arrow-down /></el-icon>
                        </el-button>
                        <template #dropdown>
                            <el-dropdown-menu >
                            <el-dropdown-item class="variety">Writing Instructions</el-dropdown-item>
                            <el-dropdown-item class="focus">• Pens</el-dropdown-item>
                            <el-dropdown-item>Pen 1</el-dropdown-item>
                            <el-dropdown-item class="focus">• Pencils</el-dropdown-item>
                            <el-dropdown-item>Pencil 1</el-dropdown-item>
                            </el-dropdown-menu>
                        </template>
                    </el-dropdown>
                </el-menu-item>
                <el-menu-item index="2" style="border:none;">Hot Products</el-menu-item>
                <el-menu-item index="3" style="border:none;">Brands</el-menu-item>
                <el-menu-item index="4" style="border:none;">Sourcing</el-menu-item>
                <el-menu-item index="5" style="border:none;">Clearance</el-menu-item>
                <el-menu-item index="6" style="border:none;">Eco Friendly</el-menu-item>
                <el-menu-item index="7" style="border:none;">About Us</el-menu-item>
            </el-menu>
        </el-col>
        <el-col :xs="10" :sm="4" :lg="4" class="callcenter">
            <img src="/callcenter.png"/>
            <span >1800 592 211     
            <br/>
            <div>24/7 Support Center</div>
            </span>
        </el-col>
    </el-row>
</template>

<style lang="scss" scoped>
.callcenter{
    font-weight: 400;
    color: #000;
    font-size: 13px;
    vertical-align: center;
}
.callcenter span {
    color: #e61b23;
    display: inline-block;
    font-size:max(15px,calc(100vw * 30 / 1920));
    font-family: 'Poppins', sans-serif;
    font-weight: 900;
    line-height: 1em;
    padding: 20px 0;
    letter-spacing: -0.5px;
}
.callcenter img {
    vertical-align:60%;
    height: calc(100vw * 40 / 1920);
    width: calc(100vw * 40 / 1920);
    max-width: 100%;
    min-width: 20px;
    min-height: 20px;
    margin-right: 5px;
}
.callcenter div {
    display: inline-block;
    color: #000;
    font-weight: 100;
    font-size:max(12px,calc(100vw * 18 / 1920));
    margin-top: 1px;
    margin-left: 5px;
}
.el-dropdown {
  margin-left: 15px;
}
.el-dropdown-link {
  cursor: pointer;
  color: var(--el-color-primary);
  display: flex;
  align-items: center;
}
.el-dropdown .el-button {
    height: max(25px,calc(100vw * 40 / 1280));
    width: max(190px,calc(100vw * 270 / 1920));
    background-color:#207BC1;
    border-color:#207BC1;
}
.el-menu-item {
    font-size: max(15px,calc(100vw * 23 / 1920));
    font-weight: 500;
}
.el-dropdown-menu {
    height: auto;
    width: max(100px,calc(100vw * 270 / 1920));
}
</style>
<style lang="scss">
.variety {
    font-size: max(14px,calc(100vw * 23 / 1920));
    font-weight: 900;

    color: #207BC1
}
.focus {
    font-weight: 700;
    font-size: max(12px,calc(100vw * 20 / 1920));
}
</style>