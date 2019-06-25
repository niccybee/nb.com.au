<template>
  <main>
    <section class="fold">
      <div class="content-container flex center flex-col">
        <h1>Work</h1>
        <div class="work-display rellax">
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
          <h2>Second Article Heading</h2>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus, harum exercitationem rerum nostrum nobis eos. Eveniet quos incidunt ex itaque quas dignissimos veritatis maxime, assumenda quia ipsam. Dignissimos, quas libero.</p>
        </div>
        <!-- <article class="flex center flex-col">
          
        </article>-->
      </div>
    </section>
  </main>
</template>

<script>
import Rellax from "rellax";
export default {
  mounted() {
    var laxWorkDisplay = new Rellax(".work-display");
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
}
.work-item {
  height: 8rem;
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
</style>
