<template>
  <header>
    <NavbarComponent />
  </header>
  <section class="container-fluid blink">
    <div class="row mobile justify-content-center pt-3">
      <div class="col-12 d-flex flex-column align-items-center">
        <h2 class="text-retro fs-lg d-flex letter-space">ABOUT ME</h2>
        <span class="divider"></span>
      </div>
      <div class="col-lg-5 col-md-6 col-sm-12 d-flex flex-column align-items-center pt-5 fade-in">
        <img class="p-4 code-works-logo mobile"
          src="https://codeworks.blob.core.windows.net/public/assets/img/cw-logo-circle.png" alt="Boise CodeWorks Logo">
        <h3 class="text-retro fs-md pt-3"><span class="material-symbols-outlined text-retro fs-lg">
            school
          </span> Class of Fall '22</h3>
      </div>
      <div class="col-lg-5 col-md-12 col-sm-12 text-retro fs-md my-3 letter-space fade-in">
        <p class="paragraph-fs paragraph text-shadow pt-4"> &nbsp&nbsp I discoverd software development
          from
          a simple Udemy course on javascript and after that I knew it was what I wanted to pursue. After a grueling
          13-week software development bootcamp with CodeWorks Boise, I have built the confidence and skills needed to
          build web
          applications. I primarily spend my software development time honing my Vue.js, Firbase, and web design skills.
          <br>
          &nbsp&nbsp Presently, I am a master's student enrolled in Boise State Universities cyber
          operations and
          resilience program. My intention is to pursue a career in software penetration testing as a cybersecurity
          analyst and/or cybersecurity engineer.
        </p>
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
.blink {
  animation: blinker .1s step-start 2;
}

@keyframes blinker {
  50% {
    opacity: 0;
  }
}

.code-works-logo {
  border: solid #33ff00 2px;
  background: linear-gradient(#33ff003e, #33ff003e);
}

.mobile {
  margin-bottom: 2rem;
}

@media (max-width: 768px) {
  .code-works-logo {
    max-width: 17rem;
    margin-bottom: .25rem;
  }

  .paragraph-fs {
    font-size: 16px;
  }

  .mobile {
    margin-bottom: .25rem;
  }
}
</style>