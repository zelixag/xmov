<template>
  <div class="div-wrapper-subsection">
    <div v-for="(panel, index) in panels" :key="index" v-show="activeTab === index" class="tab-panel">
      <div v-for="(item, itemIndex) in panel" :key="itemIndex" class="frame-13">
        <div class="img-wrapper">
          <img class="img-3" :alt="item.alt" :src="item.imageSrc" />
        </div>
        <div class="frame-14">
          <img class="company-logo" alt="Company logo" src="https://c.animaapp.com/gAExYClS/img/company-logo-5.svg" />
          <div class="text-wrapper-9">{{ item.description }}</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent, PropType } from "vue";

export default defineComponent({
  name: "DivWrapperSubsection",
  props: {
    activeTab: {
      type: Number as PropType<number>,
      required: true,
    },
  },
  setup() {
    const panels = [
      [
        {
          alt: "医疗医美1",
          imageSrc: "https://c.animaapp.com/gAExYClS/img/--2025-06-06---5-29-10-1.png",
          description: "医疗医美行业案例1：通报魔珐打造了品牌数字人VIVI，批量化生产短视频内容，通过视频号，自建商城等全域传播，真正时间品销同频",
        },
        {
          alt: "医疗医美2",
          imageSrc: "https://c.animaapp.com/gAExYClS/img/--2025-06-09---1-39-13-1.png",
          description: "医疗医美行业案例2：通报魔珐打造了品牌数字人VIVI，批量化生产短视频内容，通过视频号，自建商城等全域传播，真正时间品销同频",
        },
        {
          alt: "医疗医美3",
          imageSrc: "https://c.animaapp.com/gAExYClS/img/image-25@2x.png",
          description: "医疗医美行业案例3：通报魔珐打造了品牌数字人VIVI，批量化生产短视频内容，通过视频号，自建商城等全域传播，真正时间品销同频",
        },
      ],
      // Add more panels for other tabs
      [
        {
          alt: "教育教学1",
          imageSrc: "https://c.animaapp.com/gAExYClS/img/--2025-06-06---5-29-10-1.png",
          description: "教育教学行业案例1：通过AI数字人技术，提供个性化学习体验和互动式课程内容",
        },
        {
          alt: "教育教学2",
          imageSrc: "https://c.animaapp.com/gAExYClS/img/--2025-06-09---1-39-13-1.png",
          description: "教育教学行业案例2：利用数字人助教，提高学生参与度和学习效果",
        },
      ],
      [
        {
          alt: "快销行业1",
          imageSrc: "https://c.animaapp.com/gAExYClS/img/image-25@2x.png",
          description: "快销行业案例1：数字人代言提升品牌形象，增加产品曝光度和销量",
        },
        {
          alt: "快销行业2",
          imageSrc: "https://c.animaapp.com/gAExYClS/img/--2025-06-06---5-29-10-1.png",
          description: "快销行业案例2：通过数字人直播，实现24/7不间断的产品展示和客户互动",
        },
      ],
      // Add panels for other tabs (广电行业, 公共政务, 企业培训)
    ];

    return {
      panels,
    };
  },
});
</script>

<style>
.div-wrapper-subsection {
  align-items: flex-start;
  display: flex;
  gap: 20px;
  left: 100px;
  position: absolute;
  top: 4172px;
  flex-wrap: wrap;
  width: calc(100% - 200px);
}

.tab-panel {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  width: 100%;
}

.frame-13 {
  align-items: flex-start;
  display: flex;
  flex: 0 0 calc(33.33% - 14px);
  flex-direction: column;
  gap: 20px;
  position: relative;
}

.img-wrapper {
  background-color: #bbbbbb;
  border-radius: 4px;
  height: 293px;
  overflow: hidden;
  position: relative;
  width: 100%;
}

.img-3 {
  height: 100%;
  left: 0;
  object-fit: cover;
  position: absolute;
  top: 0;
  width: 100%;
}

.frame-14 {
  align-items: flex-start;
  align-self: stretch;
  display: flex;
  flex: 0 0 auto;
  flex-direction: column;
  gap: 12px;
  padding: 0px 20px;
  position: relative;
  width: 100%;
}

.company-logo {
  height: 36px;
  position: relative;
  width: 117px;
}

.text-wrapper-9 {
  align-self: stretch;
  color: #444444;
  font-family: "PingFang SC-Regular", Helvetica;
  font-size: 14px;
  font-weight: 400;
  letter-spacing: 0;
  line-height: 24px;
  position: relative;
}
</style>
