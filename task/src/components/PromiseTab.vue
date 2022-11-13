<template>
    <el-row class="promise-container" justify="space-evenly"  align="middle">
        <el-col :xs="10" :sm="10" :md="5" class="grid-content">
            <img src="/promise1.png"/>
            <span >Express Services     
                <br/>
                <div>24/7 amazing services</div>
            </span>
        </el-col>
        <el-col :xs="10" :sm="10" :md="5" class="grid-content">
            <img src="/promise2.png" />
            <span >Free Delivery     
                <br/>
                <div>Free Delivery services</div>
            </span>
        </el-col>
        <el-col :xs="10" :sm="10" :md="5" class="grid-content">
            <img src="/promise3.png"/>
            <span >Our Guarantee    
                <br/>
                <div>Guarantee services</div>
            </span>
        </el-col>
        <el-col :xs="10" :sm="10" :md="5" class="grid-content">
            <img src="/promise4.png"/>
            <span >Best Prices & Offers     
                <br/>
                <div>Order $50 or more</div>
            </span>
        </el-col>
    </el-row>
</template>

<style lang="scss" scoped>
.el-col {
    margin: 8px;
}
.promise-container {
    padding-top: 82px;
    padding-bottom: 82px;
}
.grid-content {
  border-radius: 24px;
  min-height: 98.6px;
  background-color: #F4F6FA;
  padding: 14px 10px 14px 22px;
  height: 100%;
  vertical-align: top;
}
.grid-content img {
    vertical-align:sub;
    align-self: center;
}
.grid-content span {
    display: inline-block;
    font-family: 'Poppins', sans-serif;
    font-weight: 700;
    font-size: 16px;
    padding: 20px 0;
    letter-spacing: -0.5px;
    margin-left: 15px;
    vertical-align:super;
}
.grid-content div {
    display: inline-block;
    color: #000;
    font-weight: 100;
    font-size:12px;
    margin-top: 1px;
    margin-left: 5px;
}
</style>