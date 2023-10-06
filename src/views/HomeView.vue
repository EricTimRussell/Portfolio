<template>
  <div class="hero-vh">
    <HeroComponent />
    <SkillsComponent />
  </div>
</template>

<script>
import HeroComponent from "../components/HeroComponent.vue";
import SkillsComponent from "../components/SkillsComponent.vue";

export default {
  setup() {
    return {};
  },
  components: { HeroComponent, SkillsComponent }
}
</script>

<style scoped>

</style>
