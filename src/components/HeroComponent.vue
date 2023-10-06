<template>
  <!-- <div class="container-fluid" v-if="isLoading">
    <div class="row justify-content-center pt-5">
      <div class="console-container d-flex flex-column">
        <h1 class="text-retro">Loading Resume...</h1>
        <span class="text-secondary px-2">[C:/]Command Prompt</span>
      </div>
      <div class="inner-container text-retro flex-column d-flex">
        <span>******* PIP-OS(R) V7.1.0.8 *******</span>
        <span>ROBCO [Version 41.10]
          (c) ROBCO CORPORATION. All rights reserved.</span>
        <span class="typing-cmd-start cmd-mobile">C:\EXEC\HOLOTAPE> NPM LOAD ROM(1) </span>
        <span class="typing-cmd-middle cmd-mobile">C:\EXEC\HOLOTAPE>CMD ERROR RUN OVERRIDE</span><br>
        <span class="typing-cmd-end-start cmd-mobile">INTIALIZING HOLOTAPE PROFILE...</span>
        <span class="typing-cmd-end-1 cmd-mobile"> LOAD ROM(!): DEITRIX 303</span>
        <span class="typing-cmd-end-2 cmd-mobile"> Starting to download cache of 91.5MB</span>
        <span class="typing-cmd-end-3 cmd-mobile">Finished downloading cache in 788ms</span>
        <span class="typing-cmd-end-4 cmd-mobile">Starting to extract cache</span>
        <span class="typing-cmd-end-5 cmd-mobile">Finished extracting cache in 571ms</span>
        <span class="typing-cmd-end-6 cmd-mobile">Finished fetching cache in 1.402s</span>
        <div class="col-12 d-flex justify-content-center">
          <img class="typing-cmd-end-7 pipboy-gif" src="../assets/images/fallout-fingerGuns.gif"
            alt="pipboy finger guns gif">
        </div>
      </div>
      <button @click="skipAnimation()" class="text-retro mx-5 btn" title="Skip Animation">SKIP</button>
    </div>
  </div> -->

  <header class="sticky-top">
    <NavbarComponent />
  </header>
  <section class="container-fluid flicker-animation blink">
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
  <section class="container-fluid flicker-animation blink">
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
.blink {
  animation: blinker .1s step-start 2;
}

@keyframes blinker {
  50% {
    opacity: 0;
  }
}

.console-container {
  width: 70%;
  height: 50%;
  background-color: black;
}

.inner-container {
  width: 70%;
  height: 25rem;
  background-color: #1a1a1a;
}

.pipboy-gif {
  height: auto;
  max-width: 19rem;
  border-radius: 5px;
  padding: 1rem;
}

.typing-cmd-start {
  width: 34ch;
  animation: typing 2.5s steps(22), blinkCursor .7s step-end 5 normal;
  white-space: nowrap;
  overflow: hidden;
  font-size: 16px;
}

@keyframes typing {
  from {
    width: 0;
  }
}

@keyframes blinkCursor {
  50% {
    border-color: transparent;
    border-right: 3px solid;
  }

  to {
    border-color: transparent
  }
}

.typing-cmd-middle {
  width: 40ch;
  animation: typing-middle 4s 3.5s steps(35) normal both, blinkCursor-middle .7s 3.2s step-end 7;
  white-space: nowrap;
  overflow: hidden;
  font-size: 16px;
}

@keyframes typing-middle {
  from {
    width: 0;
  }
}

@keyframes blinkCursor-middle {
  50% {
    border-color: transparent;
    border-right: 3px solid;
  }

  to {
    border-color: transparent
  }
}

.typing-cmd-end-start {
  width: 43ch;
  animation: typing-end .1s 8.1s steps(100) both;
  white-space: nowrap;
  overflow: hidden;
  font-size: 16px;
}

@keyframes typing-end {
  from {
    width: 0;
  }
}

.typing-cmd-end-1 {
  width: 43ch;
  animation: typing-end .1s 8.5s steps(100) both;
  white-space: nowrap;
  overflow: hidden;
  font-size: 16px;
}

@keyframes typing-end {
  from {
    width: 0;
  }
}

.typing-cmd-end-2 {
  width: 43ch;
  animation: typing-end .1s 9s steps(100) both;
  white-space: nowrap;
  overflow: hidden;
  font-size: 16px;
}

@keyframes typing-end {
  from {
    width: 0;
  }
}

.typing-cmd-end-3 {
  width: 43ch;
  animation: typing-end .1s 9.5s steps(100) both;
  white-space: nowrap;
  overflow: hidden;
  font-size: 16px;
}

@keyframes typing-end {
  from {
    width: 0;
  }
}

.typing-cmd-end-4 {
  width: 43ch;
  animation: typing-end .1s 9.8s steps(100) both;
  white-space: nowrap;
  overflow: hidden;
  font-size: 16px;
}

@keyframes typing-end {
  from {
    width: 0;
  }
}

.typing-cmd-end-5 {
  width: 43ch;
  animation: typing-end .1s 10.3s steps(100) both;
  white-space: nowrap;
  overflow: hidden;
  font-size: 16px;
}

@keyframes typing-end {
  from {
    width: 0;
  }
}

.typing-cmd-end-5 {
  width: 43ch;
  animation: typing-end .1s 10.5s steps(100) both;
  white-space: nowrap;
  overflow: hidden;
  font-size: 16px;
}

@keyframes typing-end {
  from {
    width: 0;
  }
}

.typing-cmd-end-6 {
  width: 43ch;
  animation: typing-end .1s 10.7s steps(100) both;
  white-space: nowrap;
  overflow: hidden;
  font-size: 16px;
}

@keyframes typing-end {
  from {
    width: 0;
  }
}

.typing-cmd-end-7 {
  width: 43ch;
  animation: typing-end .1s 10.9s steps(100) both;
  white-space: nowrap;
  overflow: hidden;
  font-size: 16px;
}

@keyframes typing-end {
  from {
    width: 0;
  }
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

  .console-container {
    width: 95%;
    height: 50%;
  }

  .inner-container {
    width: 95%;
    height: 25rem;
  }

  .cmd-mobile {
    font-size: 12px;
  }
}
</style>
