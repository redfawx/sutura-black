<template>
  <div>
    <Navigation></Navigation>
    <nuxt>
      
    </nuxt>
    <Footer id="footer" ></Footer>
    <!-- set progressbar -->
    <!-- <vue-progress-bar></vue-progress-bar> -->
    <div class="fixed-wash d-none"></div>
    <div class="fixed-wash d-none"></div>
    <div class="fixed-wash d-none"></div>
    <div class="fixed-wash d-none"></div>
    <div class="fixed-wash d-none"></div>
    
    
  </div>
</template>

<script>
import Navigation from '../components/Navigation.vue';
import Footer from '../components/Footer.vue';

export default {
  components: {
      Navigation,
      Footer
  },
}
</script>

<style>

</style>
