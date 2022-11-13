<template>
    <el-carousel :interval="4000" type="card" height="max(330px,calc(100vw * 400 / 1280))" arrow="always" indicator-position="none" :autoplay="false">
        <el-carousel-item>
          <el-card :body-style="{ padding: '0px' }">
            <img
                src="/good1.png"
                class="image"
            />
            <div style="padding: 14px">
                <el-row>
                <el-col :sm="8" :md="6" :offset="5" class="name">
                    <span>Plastic Bags</span>
                </el-col>
                </el-row>
                <el-row>
                <el-col :sm="8" :md="6" :offset="5" class="price">
                    <span>From: $ 1.00</span>
                </el-col>
                <el-col :sm="8" :md="6" :offset="5" class="quantity">
                    <span>MOQ: 120</span>
                </el-col>
                </el-row>
                <div class="bottom">
                <el-button type="primary" plain size="large">See Products</el-button>
                </div>
            </div>
            </el-card>
        </el-carousel-item>
        <el-carousel-item >
            <el-card :body-style="{ padding: '0px' }">
            <img
                src="/good2.png"
                class="image"
            />
            <div style="padding: 14px">
                <el-row>
                <el-col :sm="8" :md="6" :offset="5" class="name">
                    <span>Jelly Bean In Bag 50g</span>
                </el-col>
                </el-row>
                <el-row>
                <el-col :sm="8" :md="6" :offset="5" class="price">
                    <span>From: $ 0.35</span>
                </el-col>
                <el-col :sm="8" :md="6" :offset="5" class="quantity">
                    <span>MOQ: 100</span>
                </el-col>
                </el-row>
                <div class="bottom">
                <el-button type="primary" plain size="large">See Products</el-button>
                </div>
            </div>
            </el-card>
        </el-carousel-item>
        <el-carousel-item>
            <el-card :body-style="{ padding: '0px' }">
            <img
                src="/good3.png"
                class="image"
            />
            <div style="padding: 14px">
                <el-row>
                <el-col :sm="8" :md="6" :offset="5" class="name">
                    <span>Miami Drink Bottle</span>
                </el-col>
                </el-row>
                <el-row>
                <el-col :sm="8" :md="6" :offset="5" class="price">
                    <span>From: $ 9.40</span>
                </el-col>
                <el-col :sm="8" :md="6" :offset="5" class="quantity">
                    <span>MOQ: 25</span>
                </el-col>
                </el-row>
                <div class="bottom">
                <el-button type="primary" plain size="large">See Products</el-button>
                </div>
            </div>
          </el-card>
        </el-carousel-item>
    </el-carousel>
    <el-row class="view-wrapper">
        <el-button>View All</el-button>
    </el-row>
</template>
<style scoped>
  .bottom {
  margin-top: 13px;
  line-height: 12px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.image {
  object-fit:scale-down;
  width: 40%;
  height: 40%;
  display: block;
  margin:0 auto;
}
.el-card {
  text-align: justify;
}
.name {
  margin-bottom: 15px;
  font-family: 'Poppins', sans-serif;
  font-weight: 700;
}
.price {
  color: #ea3a3c;
}
.quantity {
  color: rgba(63, 62, 62, 0.70);
  font-size: 14px;
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
.el-button:hover{
  background-color:#207bc1;
  color: white;
}
</style>