<template>
  <main>
    <section class="fold">
      <div class="content-container flex center flex-col">
        <h1 class="no-b-pad">Work</h1>
        <h3 class="highlights-lax rellax" data-rellax-speed="-5">Highlights</h3>
        <div class="work-display work-display-lax rellax test">
          <article class="work-item"></article>
          <article class="work-item"></article>
          <article class="work-item"></article>
          <article class="work-item"></article>
          <article class="work-item"></article>
          <article class="work-item"></article>
        </div>
      </div>
    </section>
    <PDFDownloadModal />
    <section class="fold">
      <div class="content-container flex center flex-col">
        <!-- <h1 class="no-b-pad">Work</h1> -->
        <h3>Logos</h3>
        <div class="work-display work-display-lax2 test" data-rellax-speed="2">
          <article class="work-item"></article>
          <article class="work-item"></article>
          <article class="work-item"></article>
          <article class="work-item"></article>
          <article class="work-item"></article>
          <article class="work-item"></article>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
import Rellax from "rellax";
import PDFDownloadModal from "@/components/PDFDownloadModal";

export default {
  components: {
    PDFDownloadModal
  },
  mounted() {
    var laxWorkDisplay = new Rellax(".work-display-lax");
    var laxWorkDisplay2 = new Rellax(".work-display-lax2");
    var laxHightlights = new Rellax(".highlights-lax");
  }
};
</script>

<style>
.work-display {
  width: 110%;
  /* border: 2px lightgreen solid; */
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-gap: 1rem;
  z-index: -1;
}
.work-item {
  height: 12rem;
  background: #e0ecf3;
}

/* TODO remove this and  */
/* FIX  */
.top-space {
  margin-top: 3rem;
}
/* TODO put in media queries other section */
@media only screen and (max-width: 610px) {
  .article-display {
    max-width: 90%;
  }
  .work-display {
    width: 100%;
  }
}
</style>
