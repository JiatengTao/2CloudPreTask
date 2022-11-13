<template>
    <el-row justify="center" class="QA-title">
        <h1>Find Your Answers</h1>
    </el-row>
    <el-row justify="center">
        <el-col :xs="24" :sm="12">
            <el-collapse  accordion>
                <el-collapse-item title="Question1" name="1">
                    <div>
                        FXCOPIER is the worlds most reliable remote trade copier. Its allow you to copy trades almost instantly between hundreds of MT4 accounts through the use of technology. Many of the industries leading money managers use FXCopier to easily manage multiple client accounts in tandem.
                    </div>
                </el-collapse-item>
                <el-collapse-item title="Question3" name="2">
                    <div>
                        FXCOPIER is the worlds most reliable remote trade copier. Its allow you to copy trades almost instantly between hundreds of MT4 accounts through the use of technology. Many of the industries leading money managers use FXCopier to easily manage multiple client accounts in tandem.
                    </div>
                </el-collapse-item>
                <el-collapse-item title="Question5" name="3">
                    <div>
                        FXCOPIER is the worlds most reliable remote trade copier. Its allow you to copy trades almost instantly between hundreds of MT4 accounts through the use of technology. Many of the industries leading money managers use FXCopier to easily manage multiple client accounts in tandem.
                    </div>
                </el-collapse-item>
            </el-collapse>
        </el-col>
        <el-col :xs="24" :sm="12">
            <el-collapse accordion>
                <el-collapse-item title="Question2" name="4">
                    <div>
                        FXCOPIER is the worlds most reliable remote trade copier. Its allow you to copy trades almost instantly between hundreds of MT4 accounts through the use of technology. Many of the industries leading money managers use FXCopier to easily manage multiple client accounts in tandem.
                    </div>
                </el-collapse-item>
                <el-collapse-item title="Question4" name="5">
                    <div>
                        FXCOPIER is the worlds most reliable remote trade copier. Its allow you to copy trades almost instantly between hundreds of MT4 accounts through the use of technology. Many of the industries leading money managers use FXCopier to easily manage multiple client accounts in tandem.
                    </div>
                </el-collapse-item>
                <el-collapse-item title="Question6" name="6">
                    <div>
                        FXCOPIER is the worlds most reliable remote trade copier. Its allow you to copy trades almost instantly between hundreds of MT4 accounts through the use of technology. Many of the industries leading money managers use FXCopier to easily manage multiple client accounts in tandem.
                    </div>
                </el-collapse-item>
            </el-collapse>
        </el-col>
    </el-row>
</template>

<style scoped>
.QA-title{
    margin: 30px;
}
.QA-title h1{
    color: #207bc1;
    font-weight: 400;
    font-size: 32px;
  }
.el-collapse-item{
    padding: 10px;
    margin: 20px;
    border-bottom: none;
    border: 0px;
    box-shadow: 0px 0px 15px 0px rgb(0 0 0 / 11%);
}
.el-collapse{
    --el-collapse-border-color:none;
    margin-bottom: 60px;
}
::v-deep .el-collapse-item__header{
  font-size: 18px;
  font-weight: 600;
}
::v-deep .el-collapse-item__arrow.is-active {
  transform: rotate(-90deg);
}
::v-deep .el-collapse-item__arrow {
  transform: rotate(90deg);
}
</style>
<style>

</style>