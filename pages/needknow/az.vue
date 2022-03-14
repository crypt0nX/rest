<template>
  <view class="container"
    ><view class="text1"><text>阿粥</text></view>
    <view class="text2"><text>不争不抢不管不顾不理不闹</text></view>
    <view class="text3"><text>使用须知</text></view>
    <view class="text"
      ><text
        >#&nbsp;贩卖无双亲!!!贩卖无双亲!!!贩卖无双亲!!!<br /><br />
        #&nbsp;本软件完全免费，如您通过付费渠道获取本软件，则已上当受骗!<br />
        ##&nbsp;本软件仅供学习研究使用，请勿用于任何商业非法用途，否则造成任何后果作者概不负责！！！<br />
        ##&nbsp;请大家严格遵守学校和国家的相关规定，软件仅供学习研究使用，请勿用于商业及非法用途。<br /><br />
        ###&nbsp;使用本软件即代表同意以上内容!<br /><br />
        2022-3-13&nbsp;更新内容:<br />
        -&nbsp;增加"宿舍信息"。<br />
        -&nbsp;增加"个人信息"字样。<br />
        -&nbsp;修改"如何销假?"背景颜色。<br />
        -&nbsp;修改"紧急联系人"手机号后移一位。<br />
        -&nbsp;修改"请假原因"多行顶格为与上行对齐。<br />
        -&nbsp;优化布局,细节化,更加接近真实布局。<br />
        -&nbsp;增加"需要离校"为可选项,且自动变色。<br />

        -&nbsp;修复"当前时间"与"发起申请"时间中月份小于10月不显示0的bug。<br />
        -&nbsp;不想写了...<br /> </text
    ></view>
    <view class="nav-left">
      <image src="../../static/img/az.png"></image>
    </view>
    <view class="bottom-btn1" @click="index1">确定</view></view
  >
</template>

<script>
export default {
  methods: {
    onreturn() {
      uni.redirectTo({
        url: "./index",
      });
    },
    index1: function () {
      uni.navigateTo({
        url: "../index/index",
      });
    },
  },
};
</script>

<style>
.text1 {
  position: absolute;
  top: 105px;
  left: 88px;
  z-index: 2;
  color: rgb(255, 255, 255);
}
.text2 {
  position: absolute;
  top: 130px;
  left: 88px;
  z-index: 2;
  font-size: 15px;
  color: rgb(207, 196, 196);
}
.text3 {
  position: absolute;
  top: 50px;
  left: 80%;
  z-index: 2;
  color: rgb(255, 255, 255);
}
.text {
  position: absolute;
  top: 200px;
  left: 20px;
  right: 10px;
  z-index: 2;
  line-height: 20px;
  font-size: 15px;
  letter-spacing: 1px;
  color: rgb(8, 8, 8);
}
.nav-left image {
  width: 100%;
  height: 180px;
}

.bottom-btn1 {
  position: fixed;
  bottom: 0px;
  background-color: #2f98e9;
  width: 100%;
  height: 85rpx;
  color: white;
  text-align: center;
  line-height: 85rpx;
  font-size: 32rpx;
}
</style>