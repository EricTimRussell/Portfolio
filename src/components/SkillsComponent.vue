<template>
  <section class="container-fluid page-load-flicker">
    <div class="row justify-content-center">
      <div class="col-12 d-flex justify-content-center gap-2">
        <div class="logo">
          <img title="Javascript" class="logo" src="../assets/images/Skills/javascript.png" alt="javascript logo">
        </div>
        <div class="logo">
          <img title="Bootstrap" class="logo" src="../assets/images/Skills/bootstrap.png" alt="BootStrap logo">
        </div>
        <div class="logo">
          <img title="VueJs" class="logo" src="../assets/images/Skills/vue.png" alt="vue javascript logo">
        </div>
        <div class="logo">
          <img title="Nuxtjs" class="logo" src="../assets/images/Skills/Nuxt3.png" alt="Nuxt logo">
        </div>
      </div>
      <div class="col-12 d-flex justify-content-center gap-2 py-4">
        <div class="logo">
          <img title="MySQL" class="logo" src="../assets/images/Skills/mysql.png" alt="my SQL logo">
        </div>
        <div class="logo">
          <img title="Google Firebase" class="logo" src="../assets/images/Skills/firebase_logo.png" alt="firebase logo">
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import NavbarComponent from "./NavbarComponent.vue";

export default {
  setup() {
    return {};
  },
  components: { NavbarComponent }
}
</script>

<style scoped>
.page-load-flicker {
  animation: blinker .1s step-start 3;
}

@keyframes blinker {
  50% {
    opacity: 0;
  }
}

.logo {
  width: 5rem;
  height: 5rem;
  padding: 4px;
  z-index: 4;
}

.logo:hover {
  background: linear-gradient(#33ff0076, #33ff006c);
  border-radius: 25%;
}

@media (max-width: 768px) {
  .logo{
    width: 3rem;
    height: 3rem;
  }
}
</style>