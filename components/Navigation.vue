<template>

    

    <nav class="navbar navbar-expand-lg navbar-dark px-0">
    <router-link class="navbar-brand" to="/">smt<span style="color: #ffbd00;">.</span></router-link>

      
        <div class="navbar-nav ml-auto d-none d-sm-block">
            <router-link class="nav-item nav-link mx-2" to="/works">works</router-link>

            <router-link class="nav-item nav-link mx-2" to="/about">about</router-link>
          
             <router-link class="nav-item nav-link mx-2" to="/contact">contact</router-link>
        </div>


        <div class="navbar-nav ml-auto d-block d-sm-none">
          <router-link class="nav-item nav-link mx-2" to="/">works</router-link>

            <router-link class="nav-item nav-link mx-2" to="/about">about</router-link>
          
             <router-link class="nav-item nav-link mx-2" to="/contact">contact</router-link>
        </div>


    </nav>


</template>



<script>
import TweenMax from 'gsap';

export default {
  mounted: function () {
    // TweenMax.from($('.navbar-brand'), .75, {delay: 1, x: "-=100", alpha: 0, ease: 'Power4.easeOut'});
    // TweenMax.from($('.navbar-nav'), .75, {delay: 1, x: "+=100", alpha: 0, ease: 'Power4.easeOut'});
  }
}
</script>

   
