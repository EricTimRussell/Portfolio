<template>
  <div>
    <HeroComponent />
  </div>
</template>

<script>
import AboutComponent from "../components/AboutComponent.vue";
import HeroComponent from "../components/HeroComponent.vue";
import NavbarComponent from "../components/NavbarComponent.vue";
import SkillsComponent from "../components/SkillsComponent.vue";

export default {
  setup() {
    return {};
  },
  components: { HeroComponent, AboutComponent, NavbarComponent, SkillsComponent }
}
</script>

<style scoped></style>
