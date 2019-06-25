<template>
  <header>
    <nav>
      <nuxt-link to="/">Past Work</nuxt-link>
      <nuxt-link to="/">About</nuxt-link>
      <nuxt-link to="/">CV</nuxt-link>
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
nav > a {
  color: #54798e;
  font-weight: 600;
  padding-bottom: 0.05rem;
}
nav > a:hover {
  border-bottom: solid 1px #54798e;
}
</style>
