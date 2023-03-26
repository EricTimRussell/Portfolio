<template>
  <main>
    <header class="sticky-top">
      <NavbarComponent />
    </header>
    <div>
      <HeroComponent />
    </div>
    <div class="py-5 section-height">
      <AboutComponent />
    </div>
  </main>
</template>

<script>
import AboutComponent from "../components/AboutComponent.vue";
import HeroComponent from "../components/HeroComponent.vue";
import NavbarComponent from "../components/NavbarComponent.vue";

export default {
  setup() {
    return {};
  },
  components: { HeroComponent, AboutComponent, NavbarComponent }
}
</script>

<style scoped>
.section-height {
  min-height: 75vh;
}
</style>
