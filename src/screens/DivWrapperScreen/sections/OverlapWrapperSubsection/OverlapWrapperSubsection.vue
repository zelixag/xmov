<template>
  <div class="overlap-wrapper-subsection">
    <div class="overlap">
      <div class="overlap-group">
        <img
          class="element"
          alt="Element"
          src="https://c.animaapp.com/gAExYClS/img/--1-1.png"
        />

        <div class="group">
          <div class="overlap-group-2">
            <img
              class="ellipse"
              alt="Ellipse"
              src="https://c.animaapp.com/gAExYClS/img/ellipse-9.svg"
            />

            <img
              class="img"
              alt="Ellipse"
              src="https://c.animaapp.com/gAExYClS/img/ellipse-10.svg"
            />

            <img
              class="image"
              alt="Image"
              src="https://c.animaapp.com/gAExYClS/img/image-22.png"
            />
          </div>
        </div>

        <div class="frame-3">
          <div class="frame-4">
            <img
              class="img-2"
              alt="Microphone"
              src="https://c.animaapp.com/gAExYClS/img/microphone-01.svg"
            />

            <div class="text-wrapper-4">会表达</div>
          </div>

          <div class="frame-5">
            <div class="text-wrapper-5">
              能说会道、生动表达
              <br />
              能模仿任何人的表达（声音、表情、动作）
            </div>
          </div>
        </div>

        <div class="frame-6">
          <div class="frame-4">
            <img
              class="element-2"
              alt="Message chat"
              src="https://c.animaapp.com/gAExYClS/img/message-chat-01.svg"
            />

            <div class="text-wrapper-4">可互动</div>
          </div>

          <div class="frame-5">
            <div class="text-wrapper-5">
              实时回答问题
              <br />
              多模态视频化互动
            </div>
          </div>
        </div>

        <div class="frame-7">
          <div class="frame-4">
            <div class="element-2">
              <div class="overlap-group-3">
                <div class="ellipse-2" />

                <div class="ellipse-3" />

                <div class="ellipse-4" />

                <img
                  class="vector"
                  alt="Vector"
                  src="https://c.animaapp.com/gAExYClS/img/vector-6.svg"
                />
              </div>
            </div>

            <div class="text-wrapper-4">能办事</div>
          </div>

          <div class="frame-5">
            <div class="text-wrapper-5">
              自主完成任务
              <br />
              智能体加持（LLM+知识库+插件+工作流）
            </div>
          </div>
        </div>

        <div class="frame-8">
          <div class="frame-4">
            <img
              class="element-2"
              alt="Element"
              src="https://c.animaapp.com/gAExYClS/img/---1.svg"
            />

            <div class="text-wrapper-4">有大脑</div>
          </div>

          <div class="frame-5">
            <div class="text-wrapper-5">
              有大脑、能思考
              <br />
              大模型加持（自研大模型or第三方LLM+知识库）
            </div>
          </div>
        </div>
      </div>

      <div class="frame-9">
        <div class="frame-4">
          <img
            class="img-2"
            alt="Face id"
            src="https://c.animaapp.com/gAExYClS/img/face-id-02.svg"
          />

          <div class="text-wrapper-4">有形象</div>
        </div>

        <div class="frame-5">
          <div class="text-wrapper-5">
            3D超写实
            <br />
            个性化编辑（妆容、发型、服饰、脸型）
            <br />
            个性化造人（高效率、低门槛、规模化）
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "OverlapWrapperSubsection",
});
</script>

<style>
.overlap-wrapper-subsection {
  height: 1170px;
  left: 0;
  position: absolute;
  top: 1530px;
  width: 1560px;
}

.overlap-wrapper-subsection .overlap {
  height: 1021px;
  position: relative;
  top: 130px;
}

.overlap-wrapper-subsection .overlap-group {
  height: 1021px;
  left: 0;
  position: absolute;
  top: 0;
  width: 1560px;
}

.overlap-wrapper-subsection .element {
  height: 680px;
  left: 0;
  position: absolute;
  top: 330px;
  width: 1560px;
}

.overlap-wrapper-subsection .group {
  height: 1021px;
  left: 560px;
  position: absolute;
  top: 0;
  width: 440px;
}

.overlap-wrapper-subsection .overlap-group-2 {
  height: 1021px;
  position: relative;
}

.overlap-wrapper-subsection .ellipse {
  height: 80px;
  left: 60px;
  position: absolute;
  top: 909px;
  width: 320px;
}

.overlap-wrapper-subsection .img {
  height: 120px;
  left: 0;
  position: absolute;
  top: 901px;
  width: 440px;
}

.overlap-wrapper-subsection .image {
  height: 978px;
  left: 70px;
  position: absolute;
  top: 0;
  width: 300px;
}

.overlap-wrapper-subsection .frame-3 {
  align-items: flex-start;
  display: flex;
  flex-direction: column;
  gap: 8px;
  left: 140px;
  position: absolute;
  top: 422px;
  width: 386px;
}

.overlap-wrapper-subsection .frame-4 {
  align-items: center;
  display: inline-flex;
  flex: 0 0 auto;
  gap: 12px;
  position: relative;
}

.overlap-wrapper-subsection .img-2 {
  height: 28px;
  position: relative;
  width: 28px;
}

.overlap-wrapper-subsection .text-wrapper-4 {
  color: #111111;
  font-family: "PingFang SC-Regular", Helvetica;
  font-size: 32px;
  font-weight: 400;
  letter-spacing: 0;
  line-height: normal;
  margin-top: -1.00px;
  position: relative;
  width: fit-content;
}

.overlap-wrapper-subsection .frame-5 {
  align-items: center;
  align-self: stretch;
  display: flex;
  flex: 0 0 auto;
  gap: 10px;
  justify-content: center;
  padding: 0px 0px 0px 40px;
  position: relative;
  width: 100%;
}

.overlap-wrapper-subsection .text-wrapper-5 {
  color: #444444;
  flex: 1;
  font-family: "PingFang SC-Regular", Helvetica;
  font-size: 16px;
  font-weight: 400;
  letter-spacing: 0;
  line-height: 32px;
  margin-top: -1.00px;
  position: relative;
}

.overlap-wrapper-subsection .frame-6 {
  align-items: flex-start;
  display: flex;
  flex-direction: column;
  gap: 8px;
  left: 1064px;
  position: absolute;
  top: 293px;
  width: 386px;
}

.overlap-wrapper-subsection .element-2 {
  height: 24px;
  position: relative;
  width: 24px;
}

.overlap-wrapper-subsection .frame-7 {
  align-items: flex-start;
  display: flex;
  flex-direction: column;
  gap: 8px;
  left: 1064px;
  position: absolute;
  top: 558px;
  width: 386px;
}

.overlap-wrapper-subsection .overlap-group-3 {
  height: 21px;
  left: 1px;
  position: relative;
  top: 1px;
  width: 21px;
}

.overlap-wrapper-subsection .ellipse-2 {
  border: 1.3px solid;
  border-color: #111111;
  border-radius: 3.65px;
  height: 7px;
  left: 0;
  position: absolute;
  top: 7px;
  width: 7px;
}

.overlap-wrapper-subsection .ellipse-3 {
  border: 1.3px solid;
  border-color: #111111;
  border-radius: 3.65px;
  height: 7px;
  left: 14px;
  position: absolute;
  top: 0;
  width: 7px;
}

.overlap-wrapper-subsection .ellipse-4 {
  border: 1.3px solid;
  border-color: #111111;
  border-radius: 3.65px;
  height: 7px;
  left: 14px;
  position: absolute;
  top: 14px;
  width: 7px;
}

.overlap-wrapper-subsection .vector {
  height: 15px;
  left: 6px;
  position: absolute;
  top: 3px;
  width: 9px;
}

.overlap-wrapper-subsection .frame-8 {
  align-items: flex-start;
  display: flex;
  flex-direction: column;
  gap: 8px;
  left: 140px;
  position: absolute;
  top: 671px;
  width: 386px;
}

.overlap-wrapper-subsection .frame-9 {
  align-items: flex-start;
  display: flex;
  flex-direction: column;
  gap: 8px;
  left: 140px;
  position: absolute;
  top: 173px;
  width: 386px;
}
</style>
