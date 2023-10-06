<template>
  <header class="sticky-top">
    <NavbarComponent />
  </header>
  <section class="container-fluid flicker-animation page-load-blink">
    <div class="row pt-3">
      <div class="col-4 d-flex justify-content-between header-border">
        <span class="status-bar text-retro">LVL</span>
        <span class="status-bar text-retro">5</span>
      </div>
      <div class="col-4 d-flex justify-content-center header-border">
        <span class="status-bar text-retro hero-name">Eric Russell</span>
      </div>
      <div class="col-4 d-flex justify-content-between header-border">
        <span class="status-bar text-retro">XP</span>
        <span class="status-bar text-retro">JUNIOR</span>
      </div>
    </div>
  </section>
  <section class="container-fluid flicker-animation page-load-blink">
    <div class="row p-5 fade-in">
      <div class="col-3 d-flex flex-column align-items-start">
        <span class="fs-xl border-thick text-retro mobile">CSS</span>
        <span class="fs-xl text-retro px-3 my-3 mobile">SQL</span>
        <span class="fs-xl text-retro px-3 mobile">VUE</span>
      </div>
      <div class="col-md-6 col-lg-6 col-sm-12 d-flex justify-content-center pt-5 hero-pipboy-img">
      </div>
      <div class="col-3 pt-5 mobile">
        <p class="fs-lg text-retro text-center">(12) Coffee &nbsp&nbsp A )</p>
        <p class="fs-lg text-retro text-center">80's Synthwave &nbsp&nbsp X )</p>
      </div>
      <div class="col-12 d-flex flex-column justify-content-center align-items-center rounded pt-3">
        <h3 class="hero-title">Level 5 - Full-Stack Developer</h3>
        <p class="letter-space mb-5 hero-motto">I am a
          full-stack developer
          with a particular love for Vuejs and web design.</p>
      </div>
    </div>
  </section>
</template>

<script>
import { ref, onMounted } from "vue";
import NavbarComponent from "./NavbarComponent.vue";

export default {
  setup() {
    const isLoading = ref(false);
    function pageLoading() {
      isLoading.value = true;
      setTimeout(() => {
        isLoading.value = false;
      }, 13000);
    }
    onMounted(() => {
      pageLoading();
    });
    return {
      isLoading,
      skipAnimation() {
        isLoading.value = false;
      }
    };
  },
  components: { NavbarComponent }
}
</script>

<style scoped>
.page-load-blink {
  animation: blinker .1s step-start 2;
}

@keyframes blinker {
  50% {
    opacity: 0;
  }
}

.inner-container {
  width: 70%;
  height: 25rem;
  background-color: #1a1a1a;
}

.header-border {
  border-top: 5px solid #33ff00;
  border-left: 5px solid #33ff00;
  border-right: 5px solid #33ff00;
}

.status-bar {
  font-size: 32px;
}

@media (max-width: 768px) {
  .status-bar {
    font-size: 16px;
  }

  .mobile {
    display: none;
  }
}
</style>
