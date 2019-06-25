<template>
  <div class="wrap grid grid-site" @scroll="scrollDistanceCalc">
    <HeaderNav/>
    <AsideLeft/>
    <AsideRight/>
    <div class="main block">
      <nuxt/>
    </div>
    <div class="footer block">Nicholas Benson {{year}}</div>
  </div>
</template>

<script>
import HeaderNav from "@/components/Default_Layout/HeaderNav";
import AsideLeft from "@/components/Default_Layout/AsideLeft";
import AsideRight from "@/components/Default_Layout/AsideRight";
import Rellax from "rellax";
import dayjs from "dayjs";

export default {
  components: {
    HeaderNav,
    AsideLeft,
    AsideRight
  },
  data() {
    return { scrollDistance: "" };
  },
  computed: {
    year() {
      let newDate = new Date();
      return newDate.getFullYear();
    }
  },
  mounted() {
    // var laxFpButton = new Rellax(".front-page-btn");
    // var laxCircle = new Rellax(".svg-circle");
  }
};
</script>

<style>
/* TODO create mobile resp */
@import "@/assets/css/reset.css";
@import "@/assets/css/grid.css";
@import "@/assets/css/typography.css";
@import "@/assets/css/components.css";
@import "@/assets/css/helpers.css";

.bg {
  z-index: -2;
}

/* TODO remove after testing */
.block {
  /* border: 1px solid red; */
}
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
  left: 1rem;
}
/* end */
</style>
