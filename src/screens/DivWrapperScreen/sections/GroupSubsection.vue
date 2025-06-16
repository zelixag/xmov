<template>
  <div class="group-subsection">
    <div class="group-5">
      <div class="overlap-5">
        <img
          class="group-6"
          alt="Group"
          src="https://c.animaapp.com/gAExYClS/img/group-387.png"
        />
        <div class="products-container">
          <div 
            v-for="(product, index) in products" 
            :key="index"
            :class="['product-group', { 'active-product': activeProductTab === index }]"
          >
            <div class="overlap-group-7">
              <img
                class="mask-group-2"
                alt="Mask group"
                :src="product.image"
              />
              <div class="AI-AGENT">
                {{ product.title }} <br />
                {{ product.subtitle }}
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="frame-38">
      <div class="rectangle-2"></div>
      <div class="frame-39">
        <div 
          v-for="(tab, index) in productTabs" 
          :key="index"
          :class="['tab-item', { 'tab-item-active': activeProductTab === index }]"
          @click="setActiveProductTab(index)"
        >
          {{ tab }}
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from "vue";

export default defineComponent({
  name: "GroupSubsection",
  setup() {
    const activeProductTab = ref(1); // Default to the middle tab (AI 数字人直播)
    
    const productTabs = [
      "AI 数字人视频",
      "AI 数字人直播",
      "AI 数字人交互"
    ];
    
    const products = [
      {
        title: "有言",
        subtitle: "AI VIDEO",
        image: "https://c.animaapp.com/gAExYClS/img/mask-group-2.png"
      },
      {
        title: "有灵",
        subtitle: "AI AGENT",
        image: "https://c.animaapp.com/gAExYClS/img/mask-group-1.png"
      },
      {
        title: "有光",
        subtitle: "AI LIVE",
        image: "https://c.animaapp.com/gAExYClS/img/mask-group-1.png"
      }
    ];
    
    const setActiveProductTab = (index: number) => {
      activeProductTab.value = index;
    };
    
    return {
      activeProductTab,
      productTabs,
      products,
      setActiveProductTab
    };
  }
});
</script>

<style>
.group-subsection {
  height: 790px;
  left: 124px;
  position: absolute;
  top: 564px;
  width: 1312px;
}

.group-subsection .group-5 {
  height: 650px;
  left: 0;
  position: absolute;
  top: 140px;
  width: 1312px;
}

.group-subsection .overlap-5 {
  height: 754px;
  position: relative;
  top: -47px;
  width: 1314px;
}

.group-subsection .group-6 {
  height: 754px;
  left: 181px;
  position: absolute;
  top: 0;
  width: 950px;
}

.group-subsection .products-container {
  display: flex;
  justify-content: center;
  position: absolute;
  top: 47px;
  width: 100%;
  height: 650px;
}

.group-subsection .product-group {
  height: 650px;
  width: 202px;
  opacity: 0.5;
  transition: all 0.5s ease;
  position: relative;
  margin: 0 10px;
}

.group-subsection .active-product {
  opacity: 1;
  width: 848px;
  z-index: 10;
}

.group-subsection .overlap-group-7 {
  background-color: #ffffff;
  border: 1px solid;
  border-color: #0000001a;
  border-radius: 22px;
  height: 652px;
  position: relative;
  overflow: hidden;
  transition: all 0.5s ease;
  width: 100%;
}

.group-subsection .mask-group-2 {
  height: 651px;
  left: 0;
  position: absolute;
  top: 0;
  width: 100%;
  object-fit: cover;
  transition: all 0.5s ease;
}

.group-subsection .AI-AGENT {
  color: #000000e6;
  font-family: "Roboto", Helvetica;
  font-size: 24px;
  font-style: italic;
  font-weight: 900;
  left: 16px;
  letter-spacing: 0.24px;
  line-height: 40.6px;
  position: absolute;
  top: 30px;
  width: 168px;
}

.group-subsection .frame-38 {
  align-items: flex-start;
  box-shadow: 0px 8px 20px #152b871a;
  display: inline-flex;
  flex-direction: column;
  gap: 10px;
  left: 403px;
  padding: 8px 13px;
  position: absolute;
  top: 0;
  z-index: 20;
}

.group-subsection .rectangle-2 {
  background-color: #ffffff;
  border-radius: 100px;
  height: 90px;
  left: 0;
  position: absolute;
  top: 0;
  width: 506px;
}

.group-subsection .frame-39 {
  align-items: center;
  display: inline-flex;
  flex: 0 0 auto;
  gap: 1px;
  position: relative;
  z-index: 10;
  height: 74px;
}

.group-subsection .tab-item {
  align-items: center;
  display: flex;
  justify-content: center;
  height: 52px;
  padding: 0 20px;
  position: relative;
  cursor: pointer;
  transition: all 0.3s ease;
  color: #000000;
  font-family: "PingFang SC-Regular", Helvetica;
  font-size: 16px;
  font-weight: 400;
  letter-spacing: 0;
  line-height: 24px;
  white-space: nowrap;
  margin: 0 5px;
  opacity: 0.8;
}

.group-subsection .tab-item-active {
  color: var(--variable-collection-color);
  font-family: "PingFang SC-Medium", Helvetica;
  font-weight: 500;
  opacity: 1;
  border: 1px solid var(--variable-collection-color);
  border-radius: 100px;
  background-color: #ffffff;
}
</style>
