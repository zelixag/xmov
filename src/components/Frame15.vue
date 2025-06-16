<template>
  <div :class="['frame-15', className]">
    <div class="frame-43">
      <div class="frame-44">
        <div class="text-wrapper-23">首页</div>
      </div>

      <div class="frame-45">
        <div class="text-wrapper-24">数字人产品</div>
      </div>

      <div class="frame-45">
        <div class="text-wrapper-24">核心技术</div>
      </div>

      <div class="frame-45">
        <div class="text-wrapper-24">客户案例</div>
      </div>

      <div class="frame-45">
        <div class="text-wrapper-24">行业应用</div>
      </div>

      <div class="frame-45">
        <div class="text-wrapper-24">品牌动态</div>
      </div>

      <div class="frame-45">
        <div class="text-wrapper-24">关于我们</div>
      </div>
    </div>

    <div class="union-wrapper">
      <img
        class="union"
        alt="Union"
        src="https://c.animaapp.com/gAExYClS/img/union-1.svg"
      />
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Frame15",
  props: {
    className: {
      type: String,
      default: "",
    },
  },
});
</script>

<style>
.frame-15 {
  background-color: #ffffff;
  height: 64px;
  position: relative;
  width: 1560px;
}

.frame-15 .frame-43 {
  align-items: center;
  display: inline-flex;
  gap: 40px;
  left: 471px;
  position: absolute;
  top: 10px;
}

.frame-15 .frame-44 {
  align-items: center;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-color: #111111;
  display: inline-flex;
  flex: 0 0 auto;
  gap: 10px;
  justify-content: center;
  padding: 12px 0px;
  position: relative;
}

.frame-15 .text-wrapper-23 {
  color: #111111;
  font-family: "PingFang SC-Semibold", Helvetica;
  font-size: 14px;
  font-weight: 400;
  letter-spacing: 0;
  line-height: normal;
  margin-top: -2.00px;
  position: relative;
  width: fit-content;
}

.frame-15 .frame-45 {
  align-items: center;
  border-bottom-style: solid;
  border-bottom-width: 1px;
  border-color: #ffffff;
  display: inline-flex;
  flex: 0 0 auto;
  gap: 10px;
  justify-content: center;
  padding: 12px 0px;
  position: relative;
}

.frame-15 .text-wrapper-24 {
  color: #111111;
  font-family: "PingFang SC-Regular", Helvetica;
  font-size: 14px;
  font-weight: 400;
  letter-spacing: 0;
  line-height: normal;
  margin-top: -1.00px;
  position: relative;
  width: fit-content;
}

.frame-15 .union-wrapper {
  height: 20px;
  left: 48px;
  position: absolute;
  top: 22px;
  width: 112px;
}

.frame-15 .union {
  height: 20px;
  left: 1px;
  position: absolute;
  top: 0;
  width: 110px;
}
</style>
