<template>
  <div class="slide-container">
    <div class="slide-element" :style="customStyle">
      <div class="slide-bar">
        <slot></slot>
      </div>
      <div class="slide-bar">
        <slot></slot>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "VInfiniteSlidebar",
  props: {
    slideBarStyle: {
      type: Object,
    },
    duration: {
      type: String,
      default: "15s",
    },
    direction: {
      type: String,
      default: "normal",
    },
    delay: {
      type: String,
      default: "0s",
    },
    paused: {
      type: Boolean,
      default: false,
    },
  },
  computed: {
    customStyle() {
      return {
        ...this.slideBarStyle,
        "animation-duration": this.duration,
        "animation-direction": this.direction,
        "animation-delay": this.delay,
        "animation-play-state": this.paused ? "paused" : "running",
      };
    },
  },
};
</script>

<style scoped>
@keyframes moveSlideshow {
  100% {
    transform: translateX(-50%);
  }
}
.slide-container {
  width: 100%;
  overflow: hidden;
}
.slide-element {
  transform: translate3d(0, 0, 0); /* Hey browser, please use my GPU */
  position: relative;
  overflow: hidden;
  animation-name: moveSlideshow;
  animation-iteration-count: infinite;
  animation-timing-function: linear;
  display: flex;
  width: max-content;
  min-width: 200%;
}
.slide-bar {
  width: 50%;
}
</style>
