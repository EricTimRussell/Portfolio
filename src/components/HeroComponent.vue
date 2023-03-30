<template>
  <header id="hero" class="container-fluid">
    <div class="row pt-3">
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
    <div class="row pt-5 fade-in">
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
        <h2 class="hero-name hero-animation-space anim-typewriter-name">Eric Russell</h2>
        <h3 class="hero-title hero-animation-space anim-typewriter-title">Level 5 - Full-Stack Developer</h3>
        <p class="letter-space mb-5 hero-motto hero-anim-motto anim-typewriter-motto">I am a full-stack developer
          with a particular love for Vue.js and C#</p>
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
.hero-animation-space {
  white-space: nowrap;
  overflow: hidden;
}

.hero-anim-motto {
  white-space: nowrap;
  overflow: hidden;
}

/* Animation */
.anim-typewriter-name {
  animation: typewriter-name 1s 1s normal both,
    blinkTextCursor 500ms 6 normal;
}

@keyframes typewriter-name {
  from {
    width: 0;
  }

  to {
    width: 16rem;
  }
}


@keyframes blinkTextCursor {
  from {
    border-right: #33ff00 10px solid;
  }

  to {
    border-right: transparent;
  }
}

.anim-typewriter-title {
  animation: typewriter-title 1.5s 4s normal both,
    blinkTextCursor 500ms 3.2s 8;
}

@keyframes typewriter-title {
  from {
    width: 0;
  }

  to {
    width: 36rem;
  }
}

@keyframes blinkTextCursor {
  from {
    border-right: #33ff00 10px solid;
  }

  to {
    border-right: transparent;
  }
}

.anim-typewriter-motto {
  animation: typewriter-motto 3s 8s normal both,
    blinkTextCursor 500ms 7s 10;
}

@keyframes typewriter-motto {
  from {
    width: 0;
  }

  to {
    width: 49rem;
  }
}

@keyframes blinkTextCursor {
  from {
    border-right: #33ff00 10px solid;
  }

  to {
    border-right: transparent;
  }
}


@media (max-width: 768px) {
  @keyframes typewriter-name {
    from {
      width: 0;
    }

    to {
      width: 13.5rem;
    }
  }

  @keyframes typewriter-title {
    from {
      width: 0;
    }

    to {
      width: 17rem;
    }
  }

  .anim-typewriter-motto {
    animation: none
  }

  .hero-anim-motto {
    white-space: normal;
    text-align: center;
  }

}

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