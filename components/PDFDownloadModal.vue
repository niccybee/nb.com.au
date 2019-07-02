<template>
  <section class="fold top-space">
    <div
      class="content-container flex center flex-col modal"
      :class="displayModal? displayModal : hide"
    >
      <div class="close-modal" @click="toggleModal">
        <!-- TODO replace with icon -->
        X
      </div>
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
</template>

<script>
export default {
  data() {
    return {
      displayModal: true
    };
  },
  methods: {
    toggleModal() {
      console.log(this.displayModal);
      this.displayModal = !this.displayModal;
    }
  }
};
</script>

<style>
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
.modal {
  position: relative;
  transition: opacity 0.2 ease;
}
.close-modal {
  position: absolute;
  top: 1rem;
  right: 1rem;
  cursor: pointer;
  /* TODO replace with icon */
  color: white;
  /* border: solid orange 5px; */
}
.hide {
  opacity: 0;
  display: none;
  visibility: hidden;
}
/* TODO Fix this sizing */
@media screen and (max-height: 798px) and (min-width: 610px) {
  .work-display {
    margin-bottom: 10%;
  }
  .article-display {
    padding: 0.5rem;
    margin-bottom: 2rem;
  }
}
</style>
