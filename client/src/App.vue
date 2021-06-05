<template>
  <Header />
  <router-view />
  <Footer />
</template>

<script>
import Header from '@/components/Header/Header'
import Footer from '@/components/Footer/Footer'

export default {
  components: {
    Header,
    Footer,
  },
}
</script>

<style lang="scss">
:root {
  font-size: 16px;
}

body {
  font-family: sans-serif;
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

#app {
  display: grid;
  grid-template-rows: auto auto 3.25rem;
  grid-template-areas:
    'header'
    'main'
    'footer';
}

main {
  grid-area: main;
}

.button > a,
.button > button {
  text-decoration: none;
  display: block;
  padding: 0.3125rem 0.625rem;
  text-align: center;
}
</style>
