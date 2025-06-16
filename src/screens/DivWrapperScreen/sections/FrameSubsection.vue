<template>
  <div class="frame-subsection">
    <div class="text-wrapper">让每个企业都拥有专属的AI具身智能数字人</div>
    <div class="div">有形象、会表达、有大脑、能办事的数字人员工</div>
    <div class="frame">
      <div class="div-wrapper">
        <div class="text-wrapper-2">免费体验</div>
      </div>
      <div class="frame-2">
        <div class="text-wrapper-3">探索更多产品</div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "FrameSubsection",
});
</script>

<style>
.frame-subsection {
  background-color: #ffffff;
  height: 480px;
  left: 0;
  position: absolute;
  top: 64px;
  width: 1560px;
}

.frame-subsection .text-wrapper {
  color: #111111;
  font-family: "PingFang SC-Light", Helvetica;
  font-size: 52px;
  font-weight: 300;
  left: 289px;
  letter-spacing: 0;
  line-height: normal;
  position: absolute;
  top: 119px;
}

.frame-subsection .div {
  color: #111111;
  font-family: "PingFang SC-Semibold", Helvetica;
  font-size: 16px;
  font-weight: 400;
  left: 612px;
  letter-spacing: 0;
  line-height: 26px;
  position: absolute;
  top: 212px;
  white-space: nowrap;
}

.frame-subsection .frame {
  align-items: center;
  display: inline-flex;
  gap: 16px;
  left: 572px;
  position: absolute;
  top: 288px;
}

.frame-subsection .div-wrapper {
  align-items: center;
  background-color: #111111;
  display: flex;
  gap: 10px;
  height: 48px;
  justify-content: center;
  padding: 14px 56px;
  position: relative;
  width: 200px;
}

.frame-subsection .text-wrapper-2 {
  color: #ffffff;
  font-family: "PingFang SC-Regular", Helvetica;
  font-size: 16px;
  font-weight: 400;
  letter-spacing: 1.28px;
  line-height: normal;
  margin-top: -2.00px;
  position: relative;
  width: fit-content;
}

.frame-subsection .frame-2 {
  align-items: center;
  background-color: #ffffff;
  border: 1px solid;
  border-color: #111111;
  display: flex;
  gap: 10px;
  height: 48px;
  justify-content: center;
  padding: 14px 56px;
  position: relative;
  width: 200px;
}

.frame-subsection .text-wrapper-3 {
  color: #111111;
  font-family: "PingFang SC-Regular", Helvetica;
  font-size: 16px;
  font-weight: 400;
  letter-spacing: 1.28px;
  line-height: normal;
  margin-top: -2.00px;
  position: relative;
  white-space: nowrap;
  width: fit-content;
}
</style>
