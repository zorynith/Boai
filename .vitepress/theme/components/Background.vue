<template>
  <Teleport to="body">
    <!-- 站点背景 -->
    <div class="background custom-bg">
      <img src="/background.jpg" class="cover" alt="background" />
      <div class="bg-gradient"></div>
    </div>
  </Teleport>
</template>

<script setup>
import { storeToRefs } from "pinia";
import { mainStore } from "@/store";

const store = mainStore();
const { backgroundType, backgroundUrl, themeValue } = storeToRefs(store);

// 加载失败
const coverError = (e) => {
  // 替换为透明图片
  e.target.src =
    "data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' version='1.1' width='100%25' height='100%25'%3E%3C/svg%3E";
  $message.error("背景图片加载失败，请重新设置");
};

// 加载完成
const coverLoaded = (e) => {
  const imgElement = e.target;
  // 加载完成
  imgElement.classList.add("loaded");
};
</script>

<style lang="scss" scoped>
// 新背景样式
.custom-bg {
  position: fixed;
  top: 0;
  left: 0;
  width: 100vw;
  height: 100vh;
  z-index: -2;
  background: linear-gradient(135deg, #f7f9fe 0%, #e3e8f7 100%);
  overflow: hidden;
  .cover {
    position: absolute;
    top: 0;
    left: 0;
    width: 100vw;
    height: 100vh;
    object-fit: cover;
    z-index: 1;
  filter: blur(6px);
  /* 渐变透明遮罩 */
  mask-image: linear-gradient(to bottom, rgba(204, 238, 253, 0.25) 0%, rgba(0,0,0,0.55) 100%);
  -webkit-mask-image: linear-gradient(to bottom, rgba(204, 238, 253, 0.25) 0%, rgba(0,0,0,0.55) 100%);
  }
  .bg-gradient {
    position: absolute;
    top: 0;
    left: 0;
    width: 100vw;
    height: 100vh;
    z-index: 2;
    pointer-events: none;
    background: linear-gradient(to bottom, rgba(247,249,254,0.8) 0%, rgba(247,249,254,0.2) 60%, rgba(247,249,254,0) 100%);
  }
}
</style>
