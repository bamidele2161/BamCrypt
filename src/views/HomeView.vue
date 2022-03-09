<template>
  <div class="home-container">
    <LandingPage />
    <FooterComponent />
  </div>
</template>

<script>
// @ is an alias to /src
import FooterComponent from '@/components/FooterComponent.vue'
import LandingPage from '@/components/LandingPage.vue'

export default {
  name: 'HomeView',
  components: {
    LandingPage,
    FooterComponent
  }
}
</script>
