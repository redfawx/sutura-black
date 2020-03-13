<template>
  <div style="position: relative;">
    <div id="wash"></div>
    <video playsinline="" autoplay="autoplay" loop="loop" muted="muted" preload="auto" class="my-auto mx-auto w-100"><source :src="require('@/assets/home/promo.mp4')" type="video/mp4">
      Your browser does not support HTML5 video.
    </video>
  </div>
</template>

<script>
export default {
  name: "Video",
  props: {
    msg: String
  }
};
</script>

<style lang="scss" scoped>
  #wash {
    width: 100%;
    height: 100%;
    background-color: #0b0b0b;
    opacity: .5;
    position: absolute;
  }
</style>

