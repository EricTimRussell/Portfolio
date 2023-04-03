<template>
  <div class="skills-vh">
    <SkillsComponent />
  </div>
</template>

<script>
import SkillsComponent from "../components/SkillsComponent.vue";

export default {
  setup() {
    return {};
  },
  components: { SkillsComponent }
}
</script>

<style scoped>
.skills-vh {
  min-height: 110vh;
}
</style>