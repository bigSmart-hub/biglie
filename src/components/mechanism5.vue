<template>
  <div id="mechanism5">
    <img src="../assets/banner2@2x.png" alt />
    <div class="mechanism1_container">
      <!-- 左边区域 -->
      <div class="mechanism1_left">
        <!-- 优惠信息 -->
        <div class="mechanism1_discount">
          <div class="titel">
            <div></div>
            <p>限时活动</p>
          </div>
        </div>
        <div class="mechanism1_discount_content">
          <div v-for="(item,index) in 4" :key="index">
            <img src="../assets/蒙版组 2@2x.png" alt />
            <div>
              <div class="mechanism1_discount_content_title">
                <p>限时活动名称限时活动名称</p>
                <p>进行中</p>
              </div>
              <p>活动时间：2019年10月10日-2019年10月30日</p>
            </div>
          </div>
        </div>
        <div class="mechanism1_discount1">
          <div class="titel">
            <div></div>
            <p>优惠券</p>
          </div>
          <div class="mechanism1_discount1_container">
          <img src="../assets/01.png" alt v-for="(item,index) in 3" :key='index'>
          </div>
        </div>
      </div>
      <!-- 右边区域 -->
      <div class="mechanism1_right">
        <!-- 信息选项卡 -->
        <el-tabs type="border-card" class="tabs2" v-model="activeName1">
          <el-tab-pane label="机构信息" name="first">
            <div class="jigouA">
              <img src="../assets/矩形 16@2x.png" alt />
              <p>机构名称</p>
            </div>
            <div class="jigouB">
              <div>
                <p>机构服务保障:</p>
                <div>
                  <div>
                    <img src="../assets/形状 11.png" alt />
                    <p>代价保障</p>
                  </div>
                  <div>
                    <img src="../assets/形状 12.png" alt />
                    <p>教学保障</p>
                  </div>
                  <div>
                    <img src="../assets/形状 13.png" alt />
                    <p>退款保障</p>
                  </div>
                </div>
              </div>
            </div>
            <div class="jigouC">
              <div>
                <span>10</span>
                <p>课程数量</p>
              </div>
              <div>
                <span>0</span>
                <p>读报量</p>
              </div>
              <div>
                <span>51</span>
                <p>关注量</p>
              </div>
            </div>
          </el-tab-pane>
          <el-tab-pane label="学校动态" name="second">
            <div v-for="(item,index) in 4" :key="index" class="mechanism1_right_second">
              <img src="../assets/pexels-photo-716276@2x.png" alt />
              <p>学校动态标题信息学校动态标题信息</p>
            </div>
          </el-tab-pane>
        </el-tabs>
        <!-- 优惠券 -->
        <div class="echanism1_right_coupon">
          <div class="titel">
            <div></div>
            <p>优惠券</p>
          </div>
          <img src="../assets/01.png" alt />
          <img src="../assets/01.png" alt />
        </div>
        <!-- 违规信息举报 -->
        <div class="echanism1_right_report">
          <div class="titel">
            <div></div>
            <p>违规信息举报</p>
          </div>
          <p>xxxxxxxxxxxxxxxxxxxxxxxxxxxxx</p>
          <p>xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</p>
          <p>xxxxxxxxxxxxxxxxxxxxx</p>
          <p>xxxxxxxxxxxxxxx</p>
          <button>在线投诉举报</button>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      activeName: "first",
      activeName1: "first"
    };
  },
  methods: {
    handleClick(tab, event) {
      console.log(tab, event);
    }
  }
};
</script>
<style>
#mechanism5 .mechanism1_discount1_container{
    display: flex;
    justify-content: space-between;
    padding: 0 20px 30px 20px;
}
#mechanism5 .mechanism1_discount1{
    background-color: #ffffff;
    margin-top: 20px
}
#mechanism5 .mechanism1_discount_content_title {
  display: flex;
  justify-content: space-between;
}
#mechanism5 .mechanism1_discount_content_title > p:nth-child(1) {
  font-size: 20px;
  color: #666666;
}
#mechanism5 .mechanism1_discount_content_title > p:nth-child(2) {
  width: 40px;
  height: 16px;
  background-color: #2ccc5c;
  border-radius: 4px;
  font-size: 12px;
  color: #ffffff;
  text-align: center;
}
#mechanism5 .mechanism1_discount_content > div {
  margin-bottom: 40px;
}
#mechanism5 .mechanism1_discount_content > div > div > p {
  font-size: 12px;
  color: #999999;
  margin-top: 10px;
}
#mechanism5 .mechanism1_discount_content > div > div {
  height: 53px;
  background-color: #dddddd;
  margin-top: -5px;
  padding: 10px;
}
#mechanism5 .mechanism1_discount_content {
  display: flex;
  flex-wrap: wrap;
  padding: 0 20px;
  justify-content: space-between;
  width: 860px;
  background-color: #ffffff;
  border-radius: 4px;
}
#mechanism5 .mechanism1_discount_content img {
  width: 416px;
  height: 267px;
}
#mechanism5 {
  margin: 0 auto;
  width: 1200px;
  margin-top: 20px;
}
#mechanism5 .mechanism1_discount {
  display: flex;
  position: relative;
  width: 900px;
  background-color: #ffffff;
  border-radius: 4px;
  margin-top: 20px;
}
#mechanism5 .echanism1_right_report > p {
  font-size: 12px;
  letter-spacing: 1px;
  color: #666666;
  white-space: pre-wrap;
  width: 240px;
  padding: 10px 25px 0 25px;
}
#mechanism5 .echanism1_right_report > button {
  width: 240px;
  height: 36px;
  background-color: #d12d2c;
  border-radius: 4px;
  font-size: 16px;
  letter-spacing: 2px;
  color: #ffffff;
  outline: none;
  border: none;
  margin-top: 20px;
  margin-left: 20px;
}
#mechanism5 .echanism1_right_report {
  width: 280px;
  height: 356px;
  background-color: #ffffff;
  border-radius: 4px;
  margin-top: 20px;
}
#mechanism5 .echanism1_right_coupon {
  margin-top: 20px;
  width: 280px;
  height: 360px;
  background-color: #ffffff;
  border-radius: 4px;
  text-align: center;
}
#mechanism5 .echanism1_right_coupon img {
  width: 240px;
  height: 120px;
  margin-bottom: 20px;
  margin-top: 10px;
}
#mechanism5 .mechanism1_right_second {
  display: flex;
  padding: 10px;
}
#mechanism5 .mechanism1_right_second img {
  width: 94px;
  height: 71px;
}
#mechanism5 .mechanism1_right_second p {
  font-size: 14px;
  color: #999999;
  margin-left: 10px;
}
#mechanism5 .jigouC span {
  font-size: 20px;
  color: #ff7200;
}
#mechanism5 .jigouC p {
  font-size: 12px;
  color: #999999;
}
#mechanism5 .jigouC {
  display: flex;
  justify-content: space-between;
  margin-top: 20px;
}
#mechanism5 .jigouC > div {
  flex-grow: 1;
  text-align: center;
}
#mechanism5 .jigouC > div:nth-child(2) {
  border-left: 1px solid #dddddd;
  border-right: 1px solid #dddddd;
}
#mechanism5 .jigouA {
  text-align: center;
  margin-bottom: 20px;
}
#mechanism5 .jigouA > p {
  font-size: 20px;
  color: #333333;
}
#mechanism5 .jigouB {
  padding: 0 10px;
}
#mechanism5 .jigouB p {
  font-size: 12px;
  color: #999999;
}
#mechanism5 .jigouB > div > div > div {
  text-align: center;
}
#mechanism5 .jigouB > div > div {
  display: flex;
  border-bottom: 1px solid #dddddd;
  justify-content: space-between;
  margin-top: 12px;
  padding: 0 15px 10px 15px;
}
#mechanism5 .jigouB img {
  width: 30px;
  height: 30px;
}
#mechanism5 .jigouA > img {
  width: 100px;
  height: 100px;
  padding: 10px;
}
#mechanism5 .tabs2 .el-tabs__item {
  width: 140px;
  font-size: 16px;
  color: #999999;
}
#mechanism5 .mechanism1_right {
  width: 280px;
  margin-top: 20px;
}
#mechanism5 .mechanism1_container {
  display: flex;
  justify-content: space-between;
}
#mechanism5 .titel {
  height: 60px;
  display: flex;
  align-items: center;
  box-sizing: border-box;
}
#mechanism5 .titel > div {
  width: 4px;
  height: 22px;
  background-color: #d12d2c;
  border-radius: 2px;
  margin: 0 14px 0 26px;
}
#mechanism5 .titel > p {
  font-size: 20px;
  letter-spacing: 2px;
  color: #666666;
}
</style>