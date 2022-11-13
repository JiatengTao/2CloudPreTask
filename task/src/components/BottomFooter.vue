<template>
    <el-row class="footer">
        <el-col :xs="24" :sm="10" :md="6">
            <el-descriptions title="Help & Contact" column="2">
                <el-descriptions-item label="About Us"></el-descriptions-item>
                <el-descriptions-item label="Privacy Disclaimer"></el-descriptions-item>
                <el-descriptions-item label="Terms & Conditions"></el-descriptions-item>
                <el-descriptions-item label="Artwork Guidelines"></el-descriptions-item>
                <el-descriptions-item label="Branding Methods"></el-descriptions-item>
                <el-descriptions-item label="Reviews"></el-descriptions-item>
                <el-descriptions-item label="Contact Us"></el-descriptions-item>
                <el-descriptions-item label="Membership Policy"></el-descriptions-item>
                <el-descriptions-item label="Sample Policy"></el-descriptions-item>
                <el-descriptions-item label="Payment Policy"></el-descriptions-item>
            </el-descriptions>
        </el-col>
        <el-col :xs="24" :sm="14" :md="8">
            <el-descriptions title="Categories" column="3">
                <el-descriptions-item label="Writing Instruments"></el-descriptions-item>
                <el-descriptions-item label="Bags"></el-descriptions-item>
                <el-descriptions-item label="Techology"></el-descriptions-item>
                <el-descriptions-item label="Umberllas And Ponchos"></el-descriptions-item>
                <el-descriptions-item label="Persona Items"></el-descriptions-item>
                <el-descriptions-item label="Trade Show And Event"></el-descriptions-item>
                <el-descriptions-item label="Aprons & caps"></el-descriptions-item>
                <el-descriptions-item label="Office Items"></el-descriptions-item>
                <el-descriptions-item label="Overseas Souring"></el-descriptions-item>
                <el-descriptions-item label="Photoframes"></el-descriptions-item>
                <el-descriptions-item label="Clothing"></el-descriptions-item>
                <el-descriptions-item label="Confectionery"></el-descriptions-item>
                <el-descriptions-item label="Test 5489"></el-descriptions-item>
            </el-descriptions>
        </el-col>
        <el-col :xs="24" :sm="12" :md="5" class="footer-container">
            <div class="footer-title">Our Courier Service</div>
            <img src="/courier.png" style="max-width:90%; margin-top: 10px;"/>
        </el-col>
        <el-col :xs="24" :sm="12" :md="5" class="footer-container">
            <div class="footer-title">Easy Online Shopping</div>
            <el-row justify="start" align="middle" >
                <img src="freedelivery.png" style="width: 30px; height: 30px;margin-right: 5px;"/>
                <p>Free Delivery</p>
            </el-row>
            <el-row justify="start" align="middle" >
                <img src="14return.png" style="width: 30px; height: 30px;margin-right: 5px;"/>
                <p>14 Days Return</p>
            </el-row>
        </el-col>
    </el-row>
    <el-row justify="center" align="middle" class="copyright">
        <p>Copyright © 2022 Privacy Policy | Terms & Conditions</p>
    </el-row>
</template>

<style scoped>
.footer{
    background-color: #f6fbff;
    margin-top: 40px;
    padding: 30px;
}
.el-descriptions{
    padding: 10px;
}
.footer-container{
    padding: 10px;
}
.footer-title{
    color:#207bc1;
    font-size: 16px;
    font-weight: 700;
}
.copyright{
    font-size: 13px;
}
::v-deep .el-descriptions__title {
    color:#207bc1;
    font-size: 16px;
    font-weight: 700;
}
::v-deep .el-descriptions__body .el-descriptions__table .el-descriptions__cell {
    font-size: 14px;
    padding-right: 20px;
}
::v-deep .el-descriptions__body {
    background-color:transparent;
}
::v-deep .el-descriptions__body .el-descriptions__table {
    display: inline-block;
    width: 100%;
}
</style>