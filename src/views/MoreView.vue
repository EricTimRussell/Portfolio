<template>
  <div class="more-vh">
    <MoreComponent />
  </div>
</template>

<script>
import MoreComponent from "../components/MoreComponent.vue";

export default {
  setup() {
    return {};
  },
  components: { MoreComponent }
}
</script>

<style scoped>
.more-vh {
  min-height: 84.9vh;
}
</style>