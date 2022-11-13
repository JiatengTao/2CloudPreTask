<script setup>
  import socialIcons from "./icons/SocialIcons.vue"
  import Search from "./Search.vue";
</script>

<template>
    <el-row class="topbar">
      <el-col :xs="0" :sm="6" :md="4" :xl="4" style="color: #207bc1"> The Best Online Store</el-col>
      <el-col :xs="2" :sm="6" :md="13" :xl="15"></el-col>
      <el-col :xs="14" :sm="8" :md="5" :xl="3">
        <socialIcons />
      </el-col>
      <el-col :xs="8" :sm="4" :md="2" :xl="2">
        <el-icon size="16" style="margin:5px"><User /></el-icon>
        <a style=" color: black; text-decoration: none;" href="https://idirectpromo.24livehost.com/login">Login</a>
      </el-col>
    </el-row>
    <el-row :align="middle" class="subhead">
      <el-col :xs="9" :sm="9" :lg="5" class="logo">
        <el-image style="width: 100%; height: 100%" src="/logo.png" :fit="scale-down" />
      </el-col>
      <el-col :xs="0" :sm="5" :lg="3" class="prom-container">       
        <img src="/gift.png"/>
        <span >
            Over 15000 <br/>Products Online
        </span>
      </el-col>  
      <el-col :xs="0" :sm="5" :lg="3" class="prom-container">       
        <img src="/calendar.png"/>
        <span >
            20+ Years <br/>in Industry
        </span>
      </el-col> 
      <el-col :xs="0" :sm="5" :lg="4" class="prom-container">       
        <img src="/award.png"/>
        <span >
            Quality + Services <br/>Lowest Prices
        </span>
      </el-col> 
        <Search/>
      <el-col :xs="6" :sm="0"></el-col>
      <el-col :xs="9" :sm="4" :lg="3" class="topcart-container">
        <img src="/topcart.png"/>
        <span>
            0 item(s)
        </span>
      </el-col>
    </el-row>
  </template>
  
<style lang="scss" scoped>
  
  .topbar {
    border-bottom: 1px solid #f3f4f7;
    font-size: 14px;
    font-weight: 400;
    height: 40px;
    padding-top: 5px;
  }

  .subhead {
    border-bottom: 1px solid #f3f4f7;
    height: 100%;
    display:flex;
    align-items:center;
  }

  .logo img {
    margin-top:10px ;
    margin-bottom:10px ;
  }

  .prom-container {
    max-width: 100%; 
    height: 100%;
    font-weight: 400;
    color: #000;
    font-size: 13px;
    vertical-align: middle;
  }

  .prom-container img {
    vertical-align: middle;
  }

  .prom-container span {
    display: inline-block;
    vertical-align: middle;
    padding: 20px 0;
    font-size: max(10px,calc(100vw * 14 / 1280));
  }

  .searchbox-container input{
    height: 60px;
  }

  .topcart-container img {

    vertical-align: middle;
    margin-left: 20px;
  }

  .topcart-container span {
    vertical-align:middle;
    padding-left: 10px;
    font-size: 14px;
    line-height: 1;
    color: #000;
  }
</style>

  