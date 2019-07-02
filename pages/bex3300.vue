<template>
  <main>
    <section class="fold bg-blue-line">
      <article :class="fourthW ? '4d' : 'noD'">
        <div class="title-holder flex center flex-col bg-blue-line">
          <h1>BEX3300</h1>
          <img
            data-rellax-speed="-5"
            class="rellax da da1"
            src="../static/bex3300-images/down-arrow.svg"
            alt
          />
          <h2>Nic Benson</h2>
        </div>
        <div class="flex flex-col center bg-blue-line">
          <h3></h3>
          <img
            data-rellax-speed="-10"
            class="rellax da da2"
            src="../static/bex3300-images/down-arrow.svg"
            alt
          />
          <p></p>
        </div>
        <!-- Next Section -->

        <div class="flex flex-col center bg-blue-line">
          <h2></h2>
          <h3>School</h3>
          <div class="blue-ball">
            <img class="ball-image" src="../static/bex3300-images/schools.png" alt />
          </div>
        </div>

        <div class="flex flex-col center bg-blue-line pt2">
          <h3>Starting an Arts Degree</h3>
          <div class="blue-ball">
            <img class="ball-image" src="../static/bex3300-images/arts-d.jpg" alt />
          </div>
        </div>
        <div class="flex flex-col center bg-blue-line pt2">
          <h3>Changing Degrees</h3>
          <div class="blue-ball">
            <img class="ball-image" src="../static/bex3300-images/think.png" alt />
          </div>
          <img
            data-rellax-speed="3"
            class="mfc rellax"
            src="../static/bex3300-images/Group 3.png"
            alt
          />
        </div>

        <div class="flex flex-col center bg-blue-line pt2">
          <h3>Travelling</h3>
          <div class="blue-ball">
            <img class="ball-image" src="../static/bex3300-images/plane-1.jpeg" alt />
          </div>
          <img
            data-rellax-speed="1"
            class="travel-1 br100 rellax"
            src="../static/bex3300-images/travel-1.jpg"
            alt
          />
        </div>

        <div class="flex flex-col center bg-dark-blue-line pt2">
          <h2>Family & Friends</h2>
          <h3>Family</h3>
          <div class="dark-blue-ball">
            <img class="ball-image" src="../static/bex3300-images/adam-fam.jpeg" alt />
          </div>
          <img
            data-rellax-speed="2"
            class="fam-2 rellax br100"
            src="../static/bex3300-images/fam-2.jpg"
            alt
          />
        </div>
        <div class="flex flex-col center bg-dark-blue-line pt2">
          <h3>Friends</h3>
          <div class="dark-blue-ball">
            <img class="ball-image" src="../static/bex3300-images/frends.jpg" alt />
          </div>
        </div>

        <!-- Final Section -->
        <div class="flex flex-col center bg-darker-blue-line">
          <h2>Me</h2>
          <div class="darker-blue-ball">
            <img class="br100" src="../static/bex3300-images/me.jpeg" alt />
          </div>
          <p class="bg-darker-blue-line"></p>
        </div>
        <div class="bg-darker-blue-line flex center flex-col">
          <h3>Something Else...</h3>

          <img
            class="rellax ruby-1"
            data-rellax-speed="3"
            src="@/static/bex3300-images/Intersect-1.png"
            alt
          />
          <img
            class="rellax mack-1"
            data-rellax-speed="4"
            src="@/static/bex3300-images/Intersect.png"
            alt
          />
          <nuxt-link to="/space">
            <div class="btn btn-secondary bg-white" @click="changeWorld()">Fourth World</div>
          </nuxt-link>
        </div>
      </article>
    </section>
  </main>
</template>

<script>
import Rellax from "rellax";
export default {
  data() {
    return {
      fourthW: false
    };
  },
  mounted() {
    var laxArrow1 = new Rellax(".da1");
    var laxArrow2 = new Rellax(".da2");
    var laxArrow3 = new Rellax(".da3");
    var laxRuby1 = new Rellax(".ruby-1");
    var laxRuby1 = new Rellax(".mack-1");
    var laxRuby1 = new Rellax(".mfc");
    var laxTravel = new Rellax(".travel-1");
    var laxFam = new Rellax(".fam-2");
  },
  methods: {
    changeWorld() {
      this.fourthW = !this.fourthW;
    }
  }
};
</script>

<style>
.bg-white {
  background: whitesmoke;
}
footer {
  display: none;
  visibility: hidden;
}
.bg-blue-line {
  background: url("../static/bex3300-images/blue-line.svg");
  background-repeat: repeat-Y;
  background-position: 50%;
}
.bg-dark-blue-line {
  background: url("../static/bex3300-images/dark-blue-line.svg");
  background-repeat: repeat-Y;
  background-position: 50%;
}

.bg-darker-blue-line {
  background: url("../static/bex3300-images/darker-blue-line.svg");
  background-repeat: repeat-Y;
  background-position: 50%;
}

.blue-ball {
  max-width: 70%;
  min-height: 15rem;
  min-width: 15rem;
  background: #e0ecf3;
  padding: 0.5rem;
  border-radius: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}
.dark-blue-ball {
  max-width: 70%;
  min-height: 15rem;
  min-width: 15rem;
  background: #95aab8;
  padding: 0.5rem;
  border-radius: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}
.darker-blue-ball {
  max-width: 70%;
  min-height: 15rem;
  min-width: 15rem;
  background: #627a8b;
  padding: 0.5rem;
  border-radius: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}
.da {
  z-index: -2;
  position: absolute;
}
.da1 {
  width: 30%;
}
.da2 {
  top: 50%;
}

.pt2 {
  padding-top: 2rem;
}
.ruby-1 {
  position: absolute;
  left: -1rem;
  width: 20%;
}
.mack-1 {
  position: absolute;
  right: -1rem;
  width: 20%;
}
.ball-image {
  max-width: 100%;
  border-radius: 100%;
}
.mfc {
  z-index: -2;
  width: 6rem;
  height: auto;
  position: absolute;
  right: 15%;
}
.br100 {
  border-radius: 100%;
}
.travel-1 {
  width: 16rem;
  position: absolute;
  left: 5%;
}
.fam-2 {
  position: absolute;
  right: -5%;
  width: 20rem;
}
@media only screen and (max-width: 610px) {
  .aside {
    display: none;
    visibility: hidden;
  }
  article {
    padding: 1rem;
  }
  article p {
    padding: 1rem;
  }
  h1 {
    font-size: 4rem;
  }
  h2 {
    font-size: 3rem;
  }
  h3 {
    font-size: 2rem;
    padding: 1rem;
  }
  footer {
    display: none;
    visibility: hidden;
  }
  header {
    display: none;
    visibility: hidden;
  }
  .da1 {
    width: 50%;
  }
  .travel-1 {
    left: 1rem;
    width: 40%;
  }
  .fam-2 {
    width: 30%;
  }
}
</style>
