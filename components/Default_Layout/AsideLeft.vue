<template>
  <aside class="aside aside-left block flex">
    <div class="flex logo-container">
      <Logo/>
    </div>
    <div class="social-container flex center flex-col"></div>
  </aside>
</template>

<script>
import Rellax from "rellax";
import Logo from "@/components/Logo";
export default {
  components: {
    Logo
  },
  mounted() {
    // var laxLogo = new Rellax(".logo-container");
  }
};
</script>

<style>
.social-container {
  border: solid sienna1px;
}
</style>
