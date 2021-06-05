<template>
  <header id="main-site-header">
    <span id="branding">
      <Logo />
      <h1>Agape Connection</h1>
    </span>
    <Navigation />
  </header>
</template>

<script>
import Logo from './Logo.vue'
import Navigation from './Navigation.vue'

export default {
  name: 'Header',
  components: {
    Logo,
    Navigation,
  },
}
</script>

<style lang="scss">
#main-site-header {
  grid-area: header;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0.625rem;
  width: 100%;
}
</style>
