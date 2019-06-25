<template>
  <aside class="aside aside-left block flex flex-col">
    <nux-link to="/" class="flex logo-container">
      <Logo/>
    </nux-link>
    <div class="social-container flex center flex-col">
      <div class="social-icon-item email"></div>
      <div class="social-icon-item insta"></div>
      <div class="social-icon-item twit"></div>
      <div class="social-icon-item fb"></div>
    </div>
    <div class="bg-holder">
      <BgHalfCircle class="bg-half-circle"/>
      <!-- TODO clean up bg & helpers -->
    </div>
  </aside>
</template>

<script>
import Rellax from "rellax";
import Logo from "@/components/Logo";
import BgHalfCircle from "@/components/BgHalfCircle";
export default {
  components: {
    Logo,
    BgHalfCircle
  },
  mounted() {
    var laxHalfCircle = new Rellax(".bg-half-circle");
  }
};
</script>

<style>
.logo-container {
  /* TODO reformat to utility style */
  width: 100%;
  height: max-content;
  width: max-content;
  align-items: center;
  justify-content: center;
  padding: 1rem;
  position: fixed;
  top: 0;
  left: 4%;
}
.social-container {
  border: solid sienna 1px;
  position: fixed;
  width: 6rem;
  height: 12rem;
}
.social-container .email {
  background-image: url("/assets/icons/iconmonstr-email-10.svg");
}
.social-container .insta {
  background-image: url("/assets/icons/iconmonstr-email-10.svg");
}
.social-container .twit {
  background-image: url("/assets/icons/iconmonstr-twitter-4.svg");
}
.social-container .fb {
  background-image: url("/assets/icons/iconmonstr-email-10.svg");
}
.bg-half-circle {
  position: absolute;
  top: 100vh;
}
</style>
