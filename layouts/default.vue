<template>
  <div class="wrap grid grid-site">
    <div class="aside aside-left block">x</div>
    <div class="aside aside-right block">aside right</div>
    <div class="header block">HEADER SECTION</div>
    <div class="main block">
      <nuxt/>
    </div>
    <div class="footer block">Footer Section</div>
  </div>
</template>

<script>
export default {};
</script>

<style>
/* TODO create mobile resp */
@import "@/assets/css/reset.css";
@import "@/assets/css/grid.css";
@import "@/assets/css/typography.css";

main {
  min-width: 100%;
  background: green;
  padding: 0;
  margin: 0;
}
main * {
  border: yellow solid 1px;
}
</style>

