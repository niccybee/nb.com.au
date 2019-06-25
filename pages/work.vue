<template>
  <main>
    <section class="fold">
      <div class="content-container flex center flex-col">
        <h1>Work</h1>
        <div class="work-display work-display-lax rellax">
          <article class="work-item"></article>
          <article class="work-item"></article>
          <article class="work-item"></article>
          <article class="work-item"></article>
          <article class="work-item"></article>
          <article class="work-item"></article>
        </div>
      </div>
    </section>
    <section class="fold">
      <div class="content-container flex center flex-col">
        <div class="article-display">
          <h2>PDF Download Section</h2>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus, harum exercitationem rerum nostrum nobis eos. Eveniet quos incidunt ex itaque quas dignissimos veritatis maxime, assumenda quia ipsam. Dignissimos, quas libero.</p>
          <div class="flex center">
            <div class="btn btn-primary">Download</div>
          </div>
        </div>
        <!-- <article class="flex center flex-col">
          
        </article>-->
      </div>
    </section>
    <section class="fold">
      <div class="content-container flex center flex-col">
        <!-- <h1 class="no-b-pad">Work</h1> -->
        <h3>Logos</h3>
        <div class="work-display">
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
export default {
  mounted() {
    var laxWorkDisplay = new Rellax(".work-display-lax");
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
.article-display {
  width: 130%;
  padding: 2rem;
  min-height: 2rem;
  background: #54798e;
  /* TODO fix this to typeog css */
  color: white;
  text-align: center;
  /* border: 1px solid blue; */
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
