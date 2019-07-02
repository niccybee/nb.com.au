<template>
  <main>
    <section class="fold">
      <div class="flex center fill-height flex-col">
        <!-- TODO remove main-block and replace  -->
        <div class="title-holder">
          <h1 class="title">Welcome</h1>
        </div>
        <div class="bg-holder">
          <div class="bg-square rellax bg" data-rellax-speed="10">
            <!-- TODO clean up "bg" things -->
          </div>
        </div>
      </div>
    </section>
    <section id="about-me" class="fold">
      <div class="content-container flex center flex-col">
        <h2>Who Am I?</h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam corporis atque quasi? Facilis nulla quaerat nesciunt necessitatibus exercitationem, quos magni labore dolor enim fugiat quo aperiam autem nihil nisi neque.</p>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quod at autem quae veniam molestiae. Sapiente cumque deleniti sint quaerat voluptatem consequuntur aperiam? Aut, cupiditate atque quae iure quasi sapiente repellendus!</p>
      </div>
    </section>
  </main>
</template>

<script>
import Rellax from "rellax";
export default {
  components: {},
  mounted() {
    var laxSquare = new Rellax(".bg-square");
  }
};
</script>

<style>
/* TODO clean styles : containers font-colors/styles */
.fold {
  /* border: sandybrown solid 2px; */
}
.content-container {
}
.title-holder {
  width: 500px;
  height: 100px;
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
}
.title {
  padding-bottom: 2rem;
}
/* .title {
  position: absolute;
  border: solid blue 1px;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
  width: max-content; 
  } */

.bg-holder {
  width: 102px;
  position: relative;
  /* TODO Remove */
  z-index: -1;
}
.bg-square {
  width: 100px;
  height: 530px;
  top: -230px;
  position: absolute;
  background: #e0ecf3;
  z-index: -10;
}
.bg-half-circle {
  position: absolute;
  left: -100;
}
</style>
