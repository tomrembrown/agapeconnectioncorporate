<template>
  <header id="main-site-header">
    <span id="branding">
      <Logo />
      <h1>Ashroh Enterprises</h1>
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
@use '@/displaysettings.scss' as d;

#main-site-header {
  grid-area: header;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0.625rem;
  background-color: d.$footer-header-bg-color;
  color: d.$font-color-1;

  #branding {
    margin-left: 0.5rem;
    display: flex;

    h1 {
      font: {
        size: 1.125rem;
        weight: lighter;
      }
      margin-left: 0.6em;
      margin-top: 0.2em;
    }
  }

  nav {
    margin-right: 0.5rem;

    ul {
      display: flex;
      justify-content: flex-end;
      font-size: 0.875rem;
      list-style-type: none;
      margin: 0;
      padding: 0;
      overflow: auto;

      li {
        display: inline;
      }
    }
  }
}
</style>
