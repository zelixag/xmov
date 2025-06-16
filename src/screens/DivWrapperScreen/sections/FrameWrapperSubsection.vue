<template>
  <div class="frame-wrapper-subsection">
    <div class="aigc-tabs">
      <div 
        v-for="(tab, index) in aigcTabs" 
        :key="index"
        :class="['aigc-tab', { 'active-tab': activeAigcTab === index }]"
        @click="setActiveAigcTab(index)"
      >
        {{ tab.title }}
      </div>
    </div>
    
    <div class="aigc-panels">
      <div 
        v-for="(panel, index) in aigcPanels" 
        :key="index"
        v-show="activeAigcTab === index"
        class="aigc-panel"
      >
        <div :class="['panel-container', `panel-${index}`]">
          <img
            v-if="panel.image"
            :class="['panel-image']"
            :alt="panel.title"
            :src="panel.image"
          />
          <div class="rectangle" />
          <div class="frame-10">
            <div class="text-wrapper-6">{{ panel.title }}</div>
            <div class="text-wrapper-7">{{ panel.subtitle }}</div>
          </div>
          <div class="polygon-wrapper">
            <img
              class="polygon"
              alt="Polygon"
              src="https://c.animaapp.com/gAExYClS/img/polygon-1-3.svg"
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from "vue";

export default defineComponent({
  name: "FrameWrapperSubsection",
  setup() {
    const activeAigcTab = ref(0);
    
    const aigcTabs = [
      { title: "AIGC三维形象" },
      { title: "AIGC镜头" },
      { title: "AIGC文生文" }
    ];
    
    const aigcPanels = [
      {
        title: "AIGC三维形象",
        subtitle: "智能建模&职能绑定",
        image: "https://c.animaapp.com/gAExYClS/img/image-4.png"
      },
      {
        title: "AIGC镜头",
        subtitle: "文本生成3D镜头",
        image: null
      },
      {
        title: "AIGC文生文",
        subtitle: "大语言模型LLM",
        image: "https://c.animaapp.com/gAExYClS/img/image-3-1.png"
      }
    ];
    
    const setActiveAigcTab = (index: number) => {
      activeAigcTab.value = index;
    };
    
    return {
      activeAigcTab,
      aigcTabs,
      aigcPanels,
      setActiveAigcTab
    };
  }
});
</script>

<style>
.frame-wrapper-subsection {
  position: absolute;
  top: 3050px;
  left: 0;
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.aigc-tabs {
  display: flex;
  justify-content: center;
  gap: 20px;
  margin-bottom: 30px;
  z-index: 10;
}

.aigc-tab {
  padding: 10px 20px;
  background-color: #f5f5f5;
  border-radius: 8px;
  cursor: pointer;
  font-family: "PingFang SC-Medium", Helvetica;
  font-size: 18px;
  transition: all 0.3s ease;
  border: 1px solid transparent;
}

.aigc-tab.active-tab {
  background-color: #000000;
  color: #ffffff;
  border: 1px solid #ffffff;
}

.aigc-panels {
  width: 100%;
  display: flex;
  justify-content: center;
}

.aigc-panel {
  width: 100%;
  display: flex;
  justify-content: center;
}

.panel-container {
  height: 680px;
  position: relative;
  width: 320px;
  margin: 0 10px;
  transition: all 0.5s ease;
}

.panel-0 {
  width: 560px;
}

.panel-image {
  height: 680px;
  object-fit: cover;
  position: absolute;
  top: 0;
  width: 100%;
}

.rectangle {
  background-color: #00000080;
  height: 680px;
  left: 0;
  position: absolute;
  top: 0;
  width: 100%;
}

.frame-10 {
  align-items: center;
  display: flex;
  flex-direction: column;
  gap: 8px;
  left: 50%;
  transform: translateX(-50%);
  position: absolute;
  top: 574px;
  width: 206px;
}

.text-wrapper-6 {
  align-self: stretch;
  color: #ffffff;
  font-family: "PingFang SC-Medium", Helvetica;
  font-size: 24px;
  font-weight: 500;
  letter-spacing: 0;
  line-height: normal;
  margin-top: -1.00px;
  opacity: 0.6;
  position: relative;
  text-align: center;
}

.text-wrapper-7 {
  align-self: stretch;
  color: #ffffff;
  font-family: "PingFang SC-Regular", Helvetica;
  font-size: 16px;
  font-weight: 400;
  letter-spacing: 0;
  line-height: 24px;
  opacity: 0.6;
  position: relative;
  text-align: center;
}

.polygon-wrapper {
  background-color: #000000cc;
  border: 2px solid;
  border-color: #000000;
  border-radius: 40px;
  height: 64px;
  left: 50%;
  transform: translateX(-50%);
  overflow: hidden;
  position: absolute;
  top: 308px;
  width: 64px;
}

.polygon {
  height: 18px;
  left: 26px;
  position: absolute;
  top: 23px;
  width: 16px;
}

.panel-1 {
  background-image: url(https://c.animaapp.com/gAExYClS/img/image-5.png);
  background-position: 50% 50%;
  background-size: cover;
}

.panel-2 {
  background-image: url(https://c.animaapp.com/gAExYClS/img/image-7.png);
  background-position: 50% 50%;
  background-size: cover;
}
</style>
