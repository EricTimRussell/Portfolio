<template>
  <main>
    <div>
      <HeroComponent />
    </div>
    <div class="py-5 text-center">
      <AboutComponent />
    </div>
  </main>
</template>

<script>
import AboutComponent from "../components/AboutComponent.vue";
import HeroComponent from "../components/HeroComponent.vue";

export default {
  setup() {
    return {};
  },
  components: { HeroComponent, AboutComponent }
}
</script>

<style scoped>
.border-b {
  border-bottom: 3px black solid;
}
</style>
