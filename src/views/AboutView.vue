<template>
  <div class="about-view">
    <AboutComponent />
  </div>
</template>

<script>
import AboutComponent from "../components/AboutComponent.vue";

export default {
  setup() {
    return {};
  },
  components: { AboutComponent }
}
</script>

<style scoped>
.about-view {
  min-height: 93.4vh;
}
</style>