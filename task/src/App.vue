<script setup>
import TopHeader from "./components/TopHeader.vue"
import MegaMenu from "./components/MegaMenu.vue"
import MainBanner from "./components/MainBanner.vue"
import ProductTab from "./components/ProductTab.vue"
import PromiseTab from "./components/PromiseTab.vue"
import CustomerReview from "./components/CustomerReview.vue"
import AdvertisementBoard from "./components/AdvertisementBoard.vue"
import QA from "./components/QA.vue"
import BottomFooter from "./components/BottomFooter.vue"
</script>

<template>
  <body class="body">
    <header>
      <TopHeader/>
      <MegaMenu/>
    </header>
    <main>
      <MainBanner/>
      <ProductTab/>
      <PromiseTab/>
      <CustomerReview/>
      <AdvertisementBoard/>
      <QA/>
    </main>
    <footer>
      <BottomFooter/>
    </footer>
  </body>
</template>

<style lang="scss">
.body {
    width: 100%;
    min-width: 320px;
    background-color: #fff;
    color: #3f3e3e;
    font-size: 16px;
    font-weight: 400;
    font-family: 'Lato', sans-serif;
    overflow-x: hidden;
    height: auto;
    min-height: 100vh;
    line-height: 1.5;
}
:root{
    --el-menu-active-color: none;
    --el-menu-hover-text-color: red;
    --el-menu-hover-bg-color: none;
}
</style>
