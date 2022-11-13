<template>
    <el-row justify="center" align="middle" gutter="10" class="ad-title">
        <el-col span="2">
            <h2>We</h2>
        </el-col>
        <el-col span="2">
            <img src="/heart.png"/>
        </el-col>
        <el-col span="4">
            <img src="/logo2.png" />
        </el-col>
    </el-row>
    <el-row class="glossory">
        <el-col :xs="8" :sm="4">
            <img src="ad1.png"/>
        </el-col>
        <el-col :xs="8" :sm="4">
            <img src="ad2.png"/>
        </el-col>
        <el-col :xs="8" :sm="4">
            <img src="ad3.png"/>
        </el-col>
        <el-col :xs="8" :sm="4">
            <img src="ad4.png"/>
        </el-col>
        <el-col :xs="8" :sm="4">
            <img src="ad5.png"/>
        </el-col>
        <el-col :xs="8" :sm="4">
            <img src="ad6.png"/>
        </el-col>
        <el-col :xs="8" :sm="4">
            <img src="ad7.png"/>
        </el-col>
        <el-col :xs="8" :sm="4">
            <img src="ad8.png"/>
        </el-col>
        <el-col :xs="8" :sm="4">
            <img src="ad9.png"/>
        </el-col>
        <el-col :xs="8" :sm="4">
            <img src="ad10.png"/>
        </el-col>
        <el-col :xs="8" :sm="4">
            <img src="ad11.png"/>
        </el-col>
        <el-col :xs="8" :sm="4">
            <img src="ad1.png"/>
        </el-col>
    </el-row>
    <el-row>
        <el-button>View All</el-button>
    </el-row>
</template>

<style scoped>
.ad-title h2{
    font-weight: 400;
    font-size: 30px;
}
.glossory{
    display: flex;
    flex-wrap: wrap;
    margin-bottom: 30px;
}
.glossory img{
    display: inline-block;
    padding-right: 5px;
    padding-left: 5px;
    object-fit:scale-down;
    max-height: max(120px,calc(100vw * 180 / 1280));
    max-width: max(120px,calc(100vw * 180 / 1280));
    border: 1px var(--el-border-color) solid;
}
.glossory .el-col{
    position: relative;
    text-align: center;
}
.el-button{
  margin:0 auto;
  border-width: 1.5px;
  border-color: #207bc1;
  color: #207bc1;
  padding:20px 40px 20px 40px;
  background-color: white;
  text-align: center;
}
</style>