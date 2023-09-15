<template>
  <header class="sticky-top">
    <NavbarComponent />
  </header>
  <section class="container-fluid blink">
    <div class="row pt-3">
      <div class="col-12 d-flex flex-column align-items-center">
        <h1 class="text-retro d-flex letter-space">My Works</h1>
        <span class="divider"></span>
      </div>
    </div>
    <div class="row">

      <div class="col-12 text-retro d-flex flex-column align-items-center pt-5 pb-2">
        <span class="fs-lg">My Vuejs, C#/.Net Full-Stack Apps</span>
        <span class="divider"></span>
      </div>

      <div class="col-xl-4 col-md-6 col-sm-12 my-4 d-flex justify-content-center">
        <a class="riskier" href="https://github.com/EricTimRussell/riskier" target="_blank">
          <h6 class="fs-md px-3 text-retro text-retro-shadow">Riskier Full-Stack Application</h6>
        </a>
      </div>

      <div class="col-xl-4 col-md-6 col-sm-12 my-4 d-flex justify-content-center">
        <a href="https://github.com/EricTimRussell/Keeper" target="_blank">
          <div class="keepr">
            <h6 class="fs-md px-3 text-retro text-retro-shadow">Keepr Full-Stack Application</h6>
            <img src="../assets/images/WorksBG/KeeprLogo.png" class="img-fluid portfolio-img p-3" alt="">
          </div>
        </a>
      </div>

      <div class="col-12 text-retro d-flex flex-column align-items-center pt-5 pb-2">
        <span class="fs-lg">My Vuejs and NodeJs Full-Stack App</span>
        <span class="divider"></span>
      </div>
      <div class="col-xl-4 col-md-6 col-sm-12 my-4 d-flex justify-content-center">
        <a href="https://github.com/EricTimRussell/Tower" target="_blank">
          <div class="tower">
            <h6 class="fs-md px-3 text-retro text-retro-shadow">Tower Events Full-Stack Application</h6>
            <img src="../assets/images/WorksBG/Tower.png" class="img-fluid portfolio-img p-3" alt="">
          </div>
        </a>
      </div>

      <div class="col-12 text-retro d-flex flex-column align-items-center pt-5 pb-2">
        <span class="fs-lg">My Vuejs & Google Firebase Fullstack Apps</span>
        <span class="divider"></span>
      </div>
      <div class="col-xl-4 col-md-6 col-sm-12 my-4 d-flex justify-content-center">
        <a class="riskierFire" href="https://github.com/EricTimRussell/riskierFire" target="_blank">
          <h6 class="fs-md px-3 text-retro text-retro-shadow">RiskierFire Full-Stack Application</h6>
        </a>
      </div>
      <div class="col-xl-4 col-md-6 col-sm-12 my-4 d-flex justify-content-center">
        <a href="https://getoutsidephotography.com/" target="_blank">
          <div class="get-outside-photo">
            <h6 class="fs-md px-3 text-retro text-retro-shadow">Get Outside Photography Full-Stack Application</h6>
          </div>
        </a>
      </div>

      <div class="col-12 text-retro d-flex flex-column align-items-center pt-5 pb-2">
        <span class="fs-lg">My Vuejs & Laravel Fullstack App</span>
        <span class="divider"></span>
      </div>
      <div class="col-xl-4 col-md-6 col-sm-12 my-4 d-flex justify-content-center">
        <a href="https://github.com/EricTimRussell/gregslist-laravel-vue" target="_blank">
          <div class="gregs-list">
            <h6 class="fs-md px-3 text-retro text-retro-shadow">GregsList Full-stack Application</h6>
          </div>
        </a>
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
  animation: blinker .1s step-start 4;
}

@keyframes blinker {
  50% {
    opacity: 0;
  }
}

a {
  text-decoration: none;
}

.tower {
  height: 36vh;
  width: 44vh;
  border-radius: 5px;
  background-image: url("../assets/images/WorksBG/TowerBG.png");
  background-size: contain;
  box-shadow: #33ff00 5px 5px 5px 0px, #33ff00 0px 0px 5px 8px;
}

.tower:hover {
  color: #1f5297;
  text-shadow: wheat 2px 1px;
  transform: scale(1.1);
}

.keepr {
  height: 36vh;
  width: 44vh;
  border-radius: 5px;
  background-image: url("../assets/images/WorksBG/KeeprBG.png");
  background-size: contain;
  box-shadow: #33ff00 5px 5px 5px 0px, #33ff00 0px 0px 5px 8px;
}

.keepr:hover {
  color: #1f5297;
  text-shadow: wheat 2px 1px;
  transform: scale(1.1);
}

.riskier {
  height: 36vh;
  width: 44vh;
  border-radius: 5px;
  background-image: url("../assets/images/WorksBG/RiskierBG.png");
  background-size: cover;
  box-shadow: #33ff00 5px 5px 5px 0px, #33ff00 0px 0px 5px 8px;
}

.riskier:hover {
  color: #1f5297;
  text-shadow: wheat 2px 1px;
  transform: scale(1.1);
}

.riskierFire {
  height: 36vh;
  width: 44vh;
  border-radius: 5px;
  background-image: url("../assets/images/WorksBG/RiskierFire.png");
  background-size: cover;
  box-shadow: #33ff00 5px 5px 5px 0px, #33ff00 0px 0px 5px 8px;
}

.riskierFire:hover {
  color: #1f5297;
  text-shadow: wheat 2px 1px;
  transform: scale(1.1);
}

.get-outside-photo {
  height: 36vh;
  width: 44vh;
  border-radius: 5px;
  background-image: url("../assets/images/WorksBG/GetOutside-Thumbnail.png");
  background-size: cover;
  background-position: center;
  box-shadow: #33ff00 5px 5px 5px 0px, #33ff00 0px 0px 5px 8px;
}

.get-outside-photo:hover {
  color: #1f5297;
  text-shadow: wheat 2px 1px;
  transform: scale(1.1);
}

.gregs-list {
  height: 36vh;
  width: 44vh;
  border-radius: 5px;
  background-image: url("../assets/images/WorksBG/GregsListUnderConstruction.png");
  background-size: contain;
  box-shadow: #33ff00 5px 5px 5px 0px, #33ff00 0px 0px 5px 8px;
}

.gregs-list:hover {
  color: #1f5297;
  text-shadow: wheat 2px 1px;
  transform: scale(1.1);
}

.portfolio-img {
  height: 15vh;
  width: 15vh;
  display: cover;
}

.works-expand {
  -webkit-animation: works-expand 1.5s cubic-bezier(0.225, 0.600, 0.350, 1.000) both;
  animation: works-expand 1.5s cubic-bezier(0.225, 0.600, 0.350, 1.000) both;
}

@media (max-width: 1770px) {
  .tower {
    height: 30vh;
    width: 30vh;
  }

  .keepr {
    height: 30vh;
    width: 30vh;
  }

  .network {
    height: 30vh;
    width: 30vh;
  }

  .riskier {
    height: 30vh;
    width: 30vh;
  }

  .riskierFire {
    height: 30vh;
    width: 30vh;
  }

  .get-outside-photo{
    height: 30vh;
    width: 30vh;
  }

  .gregs-list{
    height: 30vh;
    width: 30vh;
  }
}
</style>