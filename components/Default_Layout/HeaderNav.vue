<template>
  <header class="block">
    <nav>
      <nuxt-link class="nav-link" to="/work">Past Work</nuxt-link>
      <nuxt-link class="nav-link" to="/#about-me">About</nuxt-link>
      <nuxt-link class="nav-link" to="/">CV</nuxt-link>
    </nav>
  </header>
</template>

<script>
export default {
  name: "HeaderNav"
};
</script>

<style scoped>
nav {
  display: flex;
  justify-content: space-around;
  padding: 2.5rem;
}
.nav-link {
  color: #54798e;
  padding-bottom: 0.05rem;
  border-bottom: 2px solid rgba(192, 192, 192, 0);
  transition: border 0.3s ease;
}
.nav-link:hover {
  border-bottom: solid 2px #54798e;
}
</style>
