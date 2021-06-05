<template>
  <main id="home">
    <HomePageGraphic />
    <div id="home__buttons" class="button">
      <router-link to="/about">About Us</router-link>
    </div>
  </main>
</template>

<script>
import HomePageGraphic from '@/components/Home/HomePageGraphic.vue'

export default {
  name: 'Home',
  components: {
    HomePageGraphic,
  },
}
</script>
