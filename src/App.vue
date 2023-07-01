<script>
import { RouterView } from 'vue-router'
import ContactMeModalComponent from "./components/ContactMeModalComponent.vue";
export default {
  setup() {
    return {};
  },
  components: { ContactMeModalComponent }
}
</script>

<template>
  <body class="crt-effect">
    <main>
      <RouterView />
      <footer class="sticky-bottom text-end">
        <button class="contact-button mx-4 mb-2" title="Contact" data-bs-toggle="modal"
          data-bs-target="#contactModal"><span class="material-symbols-outlined text-retro fs-lg">
            smartphone
          </span></button>
      </footer>
    </main>
  </body>

  <!-- Contact Modal -->
  <div class="modal fade" id="contactModal" tabindex="-1" aria-labelledby="contactModalLabel" aria-hidden="true">
    <div class="modal-dialog modal-dialog-centered">
      <div class="modal-content modal-bg">
        <div class="modal-header">
          <h1 class="modal-title fs-lg text-retro" id="contactModalLabel">Contact Me</h1>
          <button type="button" title="Close" class="modal-close text-retro" data-bs-dismiss="modal"
            aria-label="Close">X</button>
        </div>
        <div class="modal-body modal-bg">
          <ContactMeModalComponent />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
footer {
  max-height: 12.5vh;
}

.contact-button {
  padding: .5rem;
  background: #00800000;
  border: none;
  background-color: #33ff005b;
  border-radius: 50%;
}

.contact-button:hover {
  transform: scale(1.2);
}

.modal-bg {
  background-color: #202020;
}

.modal-close {
  background-color: #2d2d2d;
}

.crt-effect::before {
  content: " ";
  display: block;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  background: linear-gradient(#12101000 50%, #00000040 50%), linear-gradient(90deg, #ff00000f, #00ff0005, #0000ff0f);
  z-index: 2;
  background-size: 100% 2px, 3px 100%;
  pointer-events: none;
}

.crt-effect::after {
  content: " ";
  display: block;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  background: rgba(18, 16, 16, 0.1);
  opacity: 0;
  z-index: 2;
  pointer-events: none;
  animation: crt-flicker 0.15s infinite;
}

@keyframes crt-flicker {
  0% {
    opacity: 0.27861;
  }

  5% {
    opacity: 0.44769;
  }

  10% {
    opacity: 0.23604;
  }

  15% {
    opacity: 0.90626;
  }

  20% {
    opacity: 0.28128;
  }

  25% {
    opacity: 0.83891;
  }

  30% {
    opacity: 0.25583;
  }

  35% {
    opacity: 0.57807;
  }

  40% {
    opacity: 0.16559;
  }

  45% {
    opacity: 0.74693;
  }

  50% {
    opacity: 0.86019;
  }

  55% {
    opacity: 0.18594;
  }

  60% {
    opacity: 0.00313;
  }

  65% {
    opacity: 0.61988;
  }

  70% {
    opacity: 0.43455;
  }

  75% {
    opacity: 0.27288;
  }

  80% {
    opacity: 0.81428;
  }

  85% {
    opacity: 0.50419;
  }

  90% {
    opacity: 0.8003;
  }

  95% {
    opacity: 0.26108;
  }

  100% {
    opacity: 0.14387;
  }
}
</style>
