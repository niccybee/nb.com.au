<template>
  <aside class="aside aside-right block">
    <!-- <div class="bg circle">...</div> -->
    <div class="circle-container">
      <div class="svg-circle rellax">
        <!-- TODO fix circle rellax movement -->
        <BgCircle class="bg-circle"/>
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
  mounted() {
    var laxBgCircle = new Rellax(".svg-circle");
    // TODO fix this rellax element to a slow move
  }
};
</script>

<style>
/* TODO put in components */
.front-page-btn {
  position: fixed;
  top: 1.2rem;
  right: 4%;
  z-index: 2;
}

/* end */
/* svg circle attampt */

.svg-circle {
  position: absolute;
  top: 0;
  right: 0;
  z-index: -10;
}
</style>
