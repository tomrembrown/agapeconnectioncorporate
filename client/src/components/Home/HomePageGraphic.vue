<template>
  <div id="home__graphic">
    <div id="home__graphic__logo"><AgapeSVGLogo /></div>
    <div id="home__graphic__title"><h2>Agape Connection</h2></div>
    <div id="home__graphic__slogan"><p>Separation is an Illusion</p></div>
  </div>
</template>

<script>
import AgapeSVGLogo from '../svg/AgapeSVGLogo'

export default {
  name: 'HomePageGraphic',
  components: {
    AgapeSVGLogo,
  },
}
</script>

<style lang="scss">
@use '@/displaysettings.scss' as d;

#home__graphic {
  display: grid;
  gap: 15px;
  grid-template-columns: 15% 85%;
}

#home__graphic__logo {
  grid-row: span 2;
}

#home__graphic__title > h2 {
  color: d.$font-color-1;
}

#home__graphic__slogan > p {
  text-transform: uppercase;
  color: d.$font-color-2;
}
</style>
