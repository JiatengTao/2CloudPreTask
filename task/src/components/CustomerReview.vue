<template>
    <div class="review-container">
        <el-row justify="center">
            <el-col :xs="4" :sm="2" :lg="1.5" :offset="2">
                <img src="/quote.png"/>
            </el-col>
            <el-col :xs="18" :sm="12" :lg="8">
                <h1>What Our Customer Say</h1>
            </el-col>
        </el-row>
        <el-row>
            <el-scrollbar>
            <div class="scrollbar-flex-content">
                <p v-for="item in 1000" :key="item" class="scrollbar-demo-item">
                    <img src="/review.png" style="object-fit:fill;"/>
                </p>
            </div>
            </el-scrollbar>
        </el-row>
    </div>
  </template>
  
  <style scoped>
  .review-container{
    background-image: url(https://idirectpromo.24livehost.com/front/img/roundbg.png);
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    background-color: #fdf6ed;
    margin-bottom: 70px;
    padding-top: 70px;
    padding-bottom: 70px;
  }
  .review-container h1{
    color: #207bc1;
    font-weight: 400;
    font-size: 32px;
  }
  .scrollbar-flex-content {
    display: flex;
  }
  .scrollbar-demo-item {
    flex-shrink: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    width: 275px;
    height: 260px;
    margin: 10px;
    text-align: center;
    border-radius: 4px;
    background: var(--el-color-danger-light-9);
    color: var(--el-color-danger);
  }
  .scrollbar-demo-item img {
    width: 275px;
    height: 260px;
  }
  </style>
  