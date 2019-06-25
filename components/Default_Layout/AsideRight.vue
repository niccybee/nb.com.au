<template>
  <aside class="aside aside-right block">
    <!-- <div class="bg circle">...</div> -->
    <div class="circle-container">
      <div class="svg-circle rellax" data-rellax-speed="-3">
        <BgCircle/>
      </div>
    </div>
    <div class="contact-container">
      <nuxt-link to="/" class="btn btn-secondary front-page-btn flex center">Contact</nuxt-link>
    </div>
  </aside>
</template>

<script>
import Rellax from "rellax";
import BgCircle from "@/components/BgCircle";

export default {
  components: {
    BgCircle
  },
  mounted() {}
};
</script>

<style>
/* TODO put in components */
.front-page-btn {
  position: fixed;
  right: 2rem;
  z-index: 2;
}

/* end */
/* svg circle attampt */
.circle-container {
  position: relative;
  border: solid salmon 1px;
}
.svg-circle {
  position: absolute;
  top: 0;
  right: 0;
  z-index: -10;
}
</style>
