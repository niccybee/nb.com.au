<template>
  <aside class="aside aside-left block flex flex-col test">
    <nux-link to="/" class="flex logo-container">
      <Logo/>
    </nux-link>
    <SocialLinks/>
    <div class="bg-holder">
      <BgHalfCircle class="bg-half-circle"/>
      <!-- TODO clean up bg & helpers -->
    </div>
  </aside>
</template>

<script>
import Rellax from "rellax";
import Logo from "@/components/Logo";
import SocialLinks from "@/components/SocialLinks";
import BgHalfCircle from "@/components/BgHalfCircle";

export default {
  components: {
    Logo,
    SocialLinks,
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
  z-index: 2;
}

.bg-half-circle {
  position: absolute;
  top: 100vh;
  z-index: -2;
}
</style>
