<template>
  <div class="div-wrapper-screen" data-model-id="22:2">
    <div class="div-2">
      <Frame15 class="frame-instance" />
      <FrameSubsection />
      <OverlapWrapperSubsection />
      <GroupSubsection />
      <div class="logo-marquee">
        <div class="logo-track">
          <div class="logo-content">
            <div class="frame-46" />
            <div class="frame-47">
              <img
                class="element-5"
                alt="Element"
                src="https://c.animaapp.com/gAExYClS/img/20250610-140650-039-10@2x.png"
              />
            </div>
            <div class="frame-48">
              <img
                class="element-6"
                alt="Element"
                src="https://c.animaapp.com/gAExYClS/img/20250610-140650-039-1-3@2x.png"
              />
            </div>
            <div class="frame-49">
              <img
                class="element-7"
                alt="Element"
                src="https://c.animaapp.com/gAExYClS/img/20250610-140650-039-7@2x.png"
              />
            </div>
            <div class="frame-50">
              <img
                class="image-8"
                alt="Image"
                src="https://c.animaapp.com/gAExYClS/img/image-43@2x.png"
              />
            </div>
            <div class="frame-51">
              <img
                class="image-9"
                alt="Image"
                src="https://c.animaapp.com/gAExYClS/img/image-42@2x.png"
              />
            </div>
            <div class="frame-48">
              <img
                class="element-6"
                alt="Element"
                src="https://c.animaapp.com/gAExYClS/img/20250610-140650-039-1-3@2x.png"
              />
            </div>
            <div class="frame-52">
              <img
                class="element-8"
                alt="Element"
                src="https://c.animaapp.com/gAExYClS/img/20250610-140650-039-12@2x.png"
              />
            </div>
            <div class="frame-48">
              <img
                class="element-6"
                alt="Element"
                src="https://c.animaapp.com/gAExYClS/img/20250610-140650-039-1-3@2x.png"
              />
            </div>
            <div class="frame-53" />
            <div class="frame-48">
              <img
                class="element-6"
                alt="Element"
                src="https://c.animaapp.com/gAExYClS/img/20250610-140650-039-1-3@2x.png"
              />
            </div>
          </div>
          <div class="logo-content">
            <div class="frame-46" />
            <div class="frame-47">
              <img
                class="element-5"
                alt="Element"
                src="https://c.animaapp.com/gAExYClS/img/20250610-140650-039-10@2x.png"
              />
            </div>
            <div class="frame-48">
              <img
                class="element-6"
                alt="Element"
                src="https://c.animaapp.com/gAExYClS/img/20250610-140650-039-1-3@2x.png"
              />
            </div>
            <div class="frame-49">
              <img
                class="element-7"
                alt="Element"
                src="https://c.animaapp.com/gAExYClS/img/20250610-140650-039-7@2x.png"
              />
            </div>
            <div class="frame-50">
              <img
                class="image-8"
                alt="Image"
                src="https://c.animaapp.com/gAExYClS/img/image-43@2x.png"
              />
            </div>
            <div class="frame-51">
              <img
                class="image-9"
                alt="Image"
                src="https://c.animaapp.com/gAExYClS/img/image-42@2x.png"
              />
            </div>
            <div class="frame-48">
              <img
                class="element-6"
                alt="Element"
                src="https://c.animaapp.com/gAExYClS/img/20250610-140650-039-1-3@2x.png"
              />
            </div>
            <div class="frame-52">
              <img
                class="element-8"
                alt="Element"
                src="https://c.animaapp.com/gAExYClS/img/20250610-140650-039-12@2x.png"
              />
            </div>
            <div class="frame-48">
              <img
                class="element-6"
                alt="Element"
                src="https://c.animaapp.com/gAExYClS/img/20250610-140650-039-1-3@2x.png"
              />
            </div>
            <div class="frame-53" />
            <div class="frame-48">
              <img
                class="element-6"
                alt="Element"
                src="https://c.animaapp.com/gAExYClS/img/20250610-140650-039-1-3@2x.png"
              />
            </div>
          </div>
        </div>
      </div>
      <div class="frame-54">
        <div class="text-wrapper-25">前沿技术内核 打造行业级AI数字人</div>
        <div class="text-wrapper-26">
          基于计算机图形学和AIGC能力，打造AI驱动的3D数字人
          高质量、高效率、规模化生产
        </div>
      </div>
      <div class="frame-55">
        <div class="text-wrapper-27">超1000+家行业客户选择魔珐</div>
        <div class="text-wrapper-28">满足各行各业多场景应用需求</div>
      </div>
      <FrameWrapperSubsection />
      <div class="frame-56">
        <div
          v-for="(tab, index) in tabs"
          :key="index"
          :class="['frame-57', { 'frame-58': activeTab === index }]"
          @click="setActiveTab(index)"
        >
          <div :class="['text-wrapper-29', { 'text-wrapper-30': activeTab === index }]">
            {{ tab }}
          </div>
        </div>
      </div>
      <DivWrapperSubsection :activeTab="activeTab" />
      <DivSubsection />
      <SectionComponentNodeSubsection />
      <Frame1Subsection />
      <OverlapGroupWrapperSubsection />
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from "vue";
import Frame15 from "../components/Frame15.vue";
import DivSubsection from "./DivWrapperScreen/sections/DivSubsection/DivSubsection.vue";
import DivWrapperSubsection from "./DivWrapperScreen/sections/DivWrapperSubsection.vue";
import Frame1Subsection from "./DivWrapperScreen/sections/Frame1Subsection.vue";
import FrameSubsection from "./DivWrapperScreen/sections/FrameSubsection.vue";
import FrameWrapperSubsection from "./DivWrapperScreen/sections/FrameWrapperSubsection.vue";
import GroupSubsection from "./DivWrapperScreen/sections/GroupSubsection.vue";
import OverlapGroupWrapperSubsection from "./DivWrapperScreen/sections/OverlapGroupWrapperSubsection/OverlapGroupWrapperSubsection.vue";
import OverlapWrapperSubsection from "./DivWrapperScreen/sections/OverlapWrapperSubsection/OverlapWrapperSubsection.vue";
import SectionComponentNodeSubsection from "./DivWrapperScreen/sections/SectionComponentNodeSubsection.vue";

export default defineComponent({
  name: "DivWrapperScreen",
  components: {
    Frame15,
    DivSubsection,
    DivWrapperSubsection,
    Frame1Subsection,
    FrameSubsection,
    FrameWrapperSubsection,
    GroupSubsection,
    OverlapGroupWrapperSubsection,
    OverlapWrapperSubsection,
    SectionComponentNodeSubsection,
  },
  setup() {
    const tabs = ["医疗医美", "教育教学", "快销行业", "广电行业", "公共政务", "企业培训"];
    const activeTab = ref(0);

    const setActiveTab = (index: number) => {
      activeTab.value = index;
    };

    return {
      tabs,
      activeTab,
      setActiveTab,
    };
  },
});
</script>

<style>
.div-wrapper-screen {
  background-color: #ffffff;
  display: flex;
  flex-direction: row;
  justify-content: center;
  width: 100%;
}

.div-wrapper-screen .div-2 {
  background-color: #ffffff;
  height: 7849px;
  overflow: hidden;
  position: relative;
  width: 1560px;
}

.div-wrapper-screen .frame-instance {
  left: 0 !important;
  position: absolute !important;
  top: 0 !important;
}

.div-wrapper-screen .logo-marquee {
  overflow: hidden;
  position: absolute;
  left: 59px;
  top: 1434px;
  width: calc(100% - 118px);
  height: 32px;
}

.div-wrapper-screen .logo-track {
  display: flex;
  animation: marquee 30s linear infinite;
  width: 200%;
}

.div-wrapper-screen .logo-content {
  display: flex;
  align-items: center;
  gap: 28px;
  opacity: 0.3;
  width: 100%;
}

@keyframes marquee {
  0% {
    transform: translateX(0);
  }
  100% {
    transform: translateX(-50%);
  }
}

.div-wrapper-screen .frame-46,
.div-wrapper-screen .frame-47,
.div-wrapper-screen .frame-48,
.div-wrapper-screen .frame-49,
.div-wrapper-screen .frame-50,
.div-wrapper-screen .frame-51,
.div-wrapper-screen .frame-52,
.div-wrapper-screen .frame-53 {
  height: 32px;
  position: relative;
}

.div-wrapper-screen .frame-46 {
  background-image: url(https://c.animaapp.com/gAExYClS/img/image-41@2x.png);
  background-size: 100% 100%;
  width: 88px;
}

.div-wrapper-screen .frame-47 { width: 163px; }
.div-wrapper-screen .frame-48 { width: 100px; }
.div-wrapper-screen .frame-49 { width: 178px; }
.div-wrapper-screen .frame-50 { width: 148px; }
.div-wrapper-screen .frame-51 { width: 86px; }
.div-wrapper-screen .frame-52 { width: 52px; }
.div-wrapper-screen .frame-53 {
  background-image: url(https://c.animaapp.com/gAExYClS/img/20250610-140650-039-9@2x.png);
  background-size: 100% 100%;
  width: 92.8px;
}

.div-wrapper-screen .element-5,
.div-wrapper-screen .element-6,
.div-wrapper-screen .element-7,
.div-wrapper-screen .image-8,
.div-wrapper-screen .image-9,
.div-wrapper-screen .element-8 {
  position: absolute;
  object-fit: cover;
}

.div-wrapper-screen .element-5 { height: 28px; left: 0; top: 2px; width: 159px; }
.div-wrapper-screen .element-6 { height: 26px; left: 0; top: 3px; width: 100px; }
.div-wrapper-screen .element-7 { height: 32px; left: 0; top: 0; width: 177px; }
.div-wrapper-screen .image-8 { height: 22px; left: 2px; top: 4px; width: 143px; }
.div-wrapper-screen .image-9 { height: 31px; left: 3px; top: 1px; width: 80px; }
.div-wrapper-screen .element-8 { height: 26px; left: 2px; top: 3px; width: 48px; }

.div-wrapper-screen .frame-54 {
  align-items: center;
  display: flex;
  flex-direction: column;
  gap: 12px;
  left: 354px;
  position: absolute;
  top: 2880px;
  width: 852px;
}

.div-wrapper-screen .text-wrapper-25 {
  align-self: stretch;
  color: #111111;
  font-family: "PingFang SC-Light", Helvetica;
  font-size: 56px;
  font-weight: 300;
  letter-spacing: 0;
  line-height: normal;
  margin-top: -1.00px;
  position: relative;
  text-align: center;
}

.div-wrapper-screen .text-wrapper-26 {
  align-self: stretch;
  color: #111111;
  font-family: "PingFang SC-Semibold", Helvetica;
  font-size: 18px;
  font-weight: 400;
  letter-spacing: 0;
  line-height: 32px;
  position: relative;
  text-align: center;
}

.div-wrapper-screen .frame-55 {
  align-items: center;
  display: flex;
  flex-direction: column;
  gap: 12px;
  left: 354px;
  position: absolute;
  top: 3910px;
  width: 852px;
}

.div-wrapper-screen .text-wrapper-27 {
  align-self: stretch;
  color: #000000;
  font-family: "PingFang SC-Light", Helvetica;
  font-size: 56px;
  font-weight: 300;
  letter-spacing: 0;
  line-height: normal;
  margin-top: -1.00px;
  position: relative;
  text-align: center;
}

.div-wrapper-screen .text-wrapper-28 {
  align-self: stretch;
  color: #000000;
  font-family: "PingFang SC-Semibold", Helvetica;
  font-size: 18px;
  font-weight: 400;
  letter-spacing: 0;
  line-height: 32px;
  position: relative;
  text-align: center;
}

.div-wrapper-screen .frame-56 {
  align-items: center;
  display: inline-flex;
  gap: 8px;
  left: 376px;
  position: absolute;
  top: 4080px;
}

.div-wrapper-screen .frame-57 {
  align-items: center;
  background-color: #eeeeee;
  border-radius: 22px;
  display: inline-flex;
  flex: 0 0 auto;
  gap: 10px;
  height: 44px;
  justify-content: center;
  overflow: hidden;
  padding: 12px 36px;
  position: relative;
  cursor: pointer;
  transition: all 0.3s ease;
}

.div-wrapper-screen .text-wrapper-29 {
  color: #444444;
  font-family: "PingFang SC-Regular", Helvetica;
  font-size: 14px;
  font-weight: 400;
  letter-spacing: 0;
  line-height: 20px;
  margin-top: -1.00px;
  position: relative;
  text-align: center;
  white-space: nowrap;
  width: fit-content;
}

.div-wrapper-screen .frame-58 {
  background-color: #000000;
}

.div-wrapper-screen .text-wrapper-30 {
  color: #ffffff;
}
</style>
