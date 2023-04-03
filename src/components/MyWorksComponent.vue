<template>
  <header class="sticky-top">
    <NavbarComponent />
  </header>
  <section class="container-fluid">
    <div class="row pt-3">
      <div class="col-12 d-flex flex-column align-items-center">
        <h2 class="text-retro fs-xl d-flex letter-space">My Work</h2>
        <span class="divider"></span>
      </div>
    </div>
    <div class="row works-expand">

      <div class="col-xl-4 col-md-6 col-sm-12 my-5 d-flex justify-content-center">
        <a href="https://github.com/EricTimRussell/Tower" target="_blank">
          <div class="tower">
            <h6 class="fs-md px-3 text-retro text-retro-shadow">Tower Events Full-Stack Application</h6>
            <img src="../assets/images/WorksBG/Tower.png" class="img-fluid portfolio-img p-3" alt="">
          </div>
        </a>
      </div>

      <div class="col-xl-4 col-md-6 col-sm-12 my-5 d-flex justify-content-center">
        <a href="https://github.com/EricTimRussell/Keeper" target="_blank">
          <div class="keepr">
            <h6 class="fs-md px-3 text-retro text-retro-shadow">Keepr Full-Stack Application</h6>
            <img src="../assets/images/WorksBG/KeeprLogo.png" class="img-fluid portfolio-img p-3" alt="">
          </div>
        </a>
      </div>

      <div class="col-xl-4 col-md-6 col-sm-12 my-5 d-flex justify-content-center">
        <a href="https://github.com/EricTimRussell/Smedia" target="_blank">
          <div class="network">
            <h6 class="fs-md px-3 text-retro text-retro-shadow">The Network Vue.js</h6>
            <img src="../assets/images/WorksBG/Network.png" class="img-fluid portfolio-img-network p-3" alt="">
          </div>
        </a>
      </div>

      <div class="col-xl-4 col-md-6 col-sm-12 my-5 d-flex justify-content-center">
        <a class="riskier" href="https://github.com/EricTimRussell/riskier" target="_blank">
          <h6 class="fs-md px-3 text-retro text-retro-shadow">Riskier Full-Stack Application</h6>
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
a {
  text-decoration: none;
}

.tower {
  height: 40vh;
  width: 48vh;
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
  height: 40vh;
  width: 48vh;
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
  height: 40vh;
  width: 48vh;
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

.network {
  height: 40vh;
  width: 48vh;
  border-radius: 5px;
  background-image: url("../assets/images/WorksBG/NetworkBG.png");
  background-size: contain;
  box-shadow: #33ff00 5px 5px 5px 0px, #33ff00 0px 0px 5px 8px;
}

.network:hover {
  color: #1f5297;
  text-shadow: wheat 2px 1px;
  transform: scale(1.1);
}

.portfolio-img {
  height: 15vh;
  width: 15vh;
  display: cover;
}

.portfolio-img-network {
  height: 9vh;
  width: 30vh;
  display: cover;
}

.works-expand {
  -webkit-animation: works-expand 1.5s cubic-bezier(0.225, 0.600, 0.350, 1.000) both;
  animation: works-expand 1.5s cubic-bezier(0.225, 0.600, 0.350, 1.000) both;
}

@-webkit-keyframes works-expand {
  0% {
    opacity: 0;
  }

  15% {
    opacity: 0.15;
  }

  25% {
    opacity: 0.25;
  }

  35% {
    opacity: 0.35;
  }

  45% {
    opacity: 0.45;
  }

  55% {
    opacity: 0.55;
  }

  65% {
    opacity: 0.65;
  }

  75% {
    opacity: 0.75;
  }

  85% {
    opacity: 0.85;
  }

  95% {
    opacity: 0.95;
  }

  100% {
    opacity: 1;
  }
}

@keyframes works-expand {
  0% {
    opacity: 0;
  }

  15% {
    opacity: 0.15;
  }

  25% {
    opacity: 0.25;
  }

  35% {
    opacity: 0.35;
  }

  45% {
    opacity: 0.45;
  }

  55% {
    opacity: 0.55;
  }

  65% {
    opacity: 0.65;
  }

  75% {
    opacity: 0.75;
  }

  85% {
    opacity: 0.85;
  }

  95% {
    opacity: 0.95;
  }

  100% {
    opacity: 1;
  }
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
}
</style>