<template>
    <el-row>
        <el-col :span="24">
            <el-carousel :interval="5000" arrow="always" height="max(60px,calc(100vw * 350 / 1280))" indicator-position="none">
                <el-carousel-item v-for="item in 2" :key="item">
                    <img src="/banner.jpg" style="width:100%; height:100%; object-fit:scale-down;"/>
                </el-carousel-item>
            </el-carousel>
        </el-col>
    </el-row>
    <el-main class="slogan">
        <span>
            THE BEST PROMOTIONAL PRODUCTS
        </span>
        <h1>
            Online store in Australia
        </h1>
        <p>
            We are the team to help you to find the Right Products (WITH QUALITY) Best Prices (GUARANTEED) Direct from manufacturers
        </p>
        <p>
            More than 20 years of selling promotional products in the world Inhouse decoration services Vast range of products online, continuing to expand Professional services
        </p>
        <p>
            Over the years, we have won and surely will continue to win a great reputation of 'On-Time Delivery' from our clients. If you have an urgent job and need help, please contact us.
        </p>
    </el-main>
</template>

<style scoped>
.slogan{
    margin-top: 20px;
    margin-bottom: 20px;
    text-align:center !important;
}
.slogan span {
    color: #207bc1;
    font-size: 20px;
    text-transform: uppercase;
    font-weight: 300;
    position: relative;
    padding-bottom: 15px;
    margin-bottom: 28px;
    display: block;
}
.slogan span::after {
    background-color: #207bc1;
    width: 100px;
    height: 1px;
    content: '';
    left: 0px;
    right: 0px;
    margin: 0px auto;
    position: absolute;
    bottom: 0px;
}
.slogan h1 {
    margin-bottom: 30px;
    font-size: 34px;
}
.slogan p {
    display: block;
    font-weight: 400;
    margin-top: 0;
    margin-bottom: 1rem;
    font-size: 18px;
    letter-spacing: -0.6px;
    word-spacing: -0.5px;
}

</style>