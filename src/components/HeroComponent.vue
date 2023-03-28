<template>
  <header id="hero" class="container-fluid">
    <div class="row pt-6">
      <div class="col-4 d-flex justify-content-between header-border">
        <span class="status-bar text-retro">LVL</span>
        <span class="status-bar text-retro">5</span>
      </div>
      <div class="col-4 d-flex justify-content-between header-border">
        <span class="status-bar text-retro">HP</span>
        <span class="status-bar text-retro">95/100</span>
      </div>
      <div class="col-4 d-flex justify-content-between header-border">
        <span class="status-bar text-retro">XP</span>
        <span class="status-bar text-retro">JUNIOR</span>
      </div>
    </div>
  </header>
  <section class="container-fluid">
    <div class="row pt-5 px-3 fade-in-hero">
      <div class="col-3 d-flex flex-column align-items-start">
        <span class="fs-xl border-thick text-retro  mobile">CSS</span>
        <span class="fs-xl text-retro px-3 my-3  mobile">SQL</span>
        <span class="fs-xl text-retro px-3  mobile">VUE</span>
      </div>
      <div class="col-md-6 col-lg-6 col-sm-12 d-flex justify-content-center pt-5 hero-pipboy-img">
      </div>
      <div class="col-3 pt-5 mobile">
        <p class="fs-lg text-retro text-center">(12) Coffee &nbsp&nbsp A )</p>
        <p class="fs-lg text-retro text-center">Willpower &nbsp&nbsp X )</p>
      </div>
      <div class="col-12 d-flex flex-column justify-content-center align-items-center rounded pt-3">
        <h2 class="hero-name title-expand">Eric Russell</h2>
        <h3 class="hero-title title-expand">Level 5 - Full-Stack Developer</h3>
        <p class="letter-space pb-5 hero-motto">I am a full-stack developer with a particular
          love for
          Vuejs and
          caffeine.</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  setup() {


    return {}
  }
}
</script>

<style scoped>
.header-border {
  border-top: 5px solid #33ff00;
  border-left: 5px solid #33ff00;
  border-right: 5px solid #33ff00;
}

.pt-6 {
  padding-top: 5rem;
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

  .pt-6 {
    padding-top: 3rem;
  }
}
</style>