<template>
  <div class="works-view">
    <MyWorksComponent />
  </div>
</template>

<script>
import MyWorksComponent from "../components/MyWorksComponent.vue";

export default {
  setup() {
    return {};
  },
  components: { MyWorksComponent }
}
</script>

<style scoped>
.works-view {
  min-height: 93.4vh;
}
</style>