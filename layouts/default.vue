<template>
  <div class="wrap grid grid-site">
    <div class="aside aside-left block">Aside left</div>
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
/* reset */
body {
  margin: 0;
  padding: 0;
}
.wrap {
  width: 100vw;
}
/* TODO remove after testing */
.block {
  border: 1px solid red;
}
/* end */
.grid {
  display: grid;
  /* remove once we fill main with content */
  height: 100vh;
  /* end */
}
.grid-site {
  grid-template-columns: 18% 60% 18%;
  grid-template-rows: 1/3fr 1/3fr 1/3fr;
  grid-template-areas:
    "aside-left header aside-right"
    "aside-left main aside-right"
    "aside-left footer aside-right";
  grid-gap: 2%;
}
.aside {
  max-height: 100vh;
}
.aside-left {
  grid-area: aside-left;
}
.aside-right {
  grid-area: aside-right;
}
.main {
  grid-area: main;
  min-height: 100%;
}
.header {
  grid-area: header;
  min-height: 2rem;
  max-height: 4rem;
}
.footer {
  grid-area: footer;
  min-height: 2rem;
  max-height: 4rem;
  align-self: end;
}
/* -ms-text-size-adjust: 100%; -webkit-text-size-adjust: 100%; -moz-osx-font-smoothing: grayscale; -webkit-font-smoothing: antialiased; box-sizing: border-box; */
</style>
