

<template>



  <transition name="enter">


        <template id="page">
          <div class="home page">
            <div id="home-content" >
              <div class="row mt-md-5 pt-5 mb-5 pb-lg-5">
                <div class="cover-photo" :style="{'background-image': 'url(' + require('@/assets/case-studies/joppa-view/hero.jpg') + ')'}">
                  &nbsp;
                </div>
              </div>

              <div class="ribbon mx-0 row justify-content-between pl-4 px-md-5 no-gutters" style="background-color:#8DD9FD;">
                <h2 id="ribbon-title" class="pt-1 my-3 mx-md-5" style="font-size: 1em; font-weight: 500; color: black;">Joppa View Elementary School Team BCPS Day <span style="color: black; font-weight: 300; font-size: 1em; margin-left: .5em;">Perry Hall, Maryland</span> </h2>
                <h2 class="my-auto mx-sm-5" style="font-size: 1em; font-weight: 300; letter-spacing: .05em;"><a class="link d-none d-sm-block" style="color:black;" href="https://vimeo.com/250881723">watch video  <i class="fas fa-arrow-right"></i></a></h2>
              </div>

              <div class="page-container">
                <div class="row my-5 py-5 justify-content-around">
                  <div class="mx-auto col-12 col-lg-7 px-0 mt-2">
                      
                      <p class="font-weight-light pt-lg-0 text-left" style="font-size: 1.5em; font-weight: 100;">
                        <span class="text-left" style="color: white; font-size: 1.1em; "> 
                          QUICK WORDS
                        </span>
                        <br>
                        <span class="font-weight-light" style="color:white;">
                          Played around with ideas, and experiences from each of my clients to put together a promotional video for a local elementary school.
                          <br>
                          <br>
                          Joppa View Elementary School had a Team Blue BCPS Day to celebrate its faculty and students. This was just a fun volunteer project to help encapsulate day.
                        </span>
                      </p>
                  </div>
                </div>
                <div class="row breakout d-none d-md-block" style="">
                  <div class="embed-responsive embed-responsive-16by9">
                    <video class="embed-responsive-item" autoplay muted loop> 
                      <source :src="require('@/assets/case-studies/joppa-view/movie.webm')" type="video/webm">
                      <source :src="require('@/assets/case-studies/joppa-view/movie.mp4')" type="video/mp4">
                    </video>
                  </div>
                </div>
                
                <div class="row my-5 py-5 justify-content-center">
                  <div class="embed-responsive embed-responsive-16by9">
                    <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/lFzrZc_LgCs?rel=0" allowfullscreen></iframe>
                  </div>
                </div>

                <div class="row py-5 px-5 breakout justify-content-center" style="background-color: white;">
                  <div class="px-5 my-auto col-12" style="background-position: 100% 27%; " >
                    <img style="max-width: 100%;" :src="require('@/assets/case-studies/joppa-view/stat.png')" >
                  </div>
                </div>
                
                <div class="row justify-content-center mt-5 mb-lg-3 pt-5">
                  <h3 class="text-white">See more of our work!</h3>
                </div>
                <div class="row justify-content-around py-5 mt-lg-5">
                  <router-link to="/callie-tomblin"
                  :style="{ backgroundImage: 'url(' + require('@/assets/emc-mobile.jpg') + ')' }"
                  style="min-height: 400px; background-color: mintcream; min-width: 400px; background-size: cover; background-position: center; " 
                  class="col-4 no-dec px-5 my-5 my-lg-0"
                  >
                    <div style="position: absolute; left: 0; right: 0; background-color: #BBC5A1; width: 100%; height: 100%; opacity: .85;"></div>
                    <h2 class="text-white pt-5 mt-4 font-weight-bolder" style="position: relative;">EMC Performing Arts Stuido</h2>
                    <p class="font-weight-light text-white" style="z-index: 100; position: relative; font-size: 1.2em !important;">
                      Creating digital content for a website and social media
                    </p>
                    <button class="mx-auto text-center d-block mb-5" style="position: relative; background: none; color: white; border: solid 2px #fbbc00; padding: 0.5em 1em;">View Work</button>
                  </router-link>

                  <router-link to="/callie-tomblin"
                  :style="{ backgroundImage: 'url(' + require('@/assets/emc-mobile.jpg') + ')' }"
                  style="min-height: 400px; background-color: mintcream; min-width: 400px; background-size: cover; background-position: center; " 
                  class="col-4 no-dec px-5 my-5 my-lg-0"
                  >
                    <div style="position: absolute; left: 0; right: 0; background-color: #BBC5A1; width: 100%; height: 100%; opacity: .85;"></div>
                    <h2 class="text-white pt-5 mt-4 font-weight-bolder" style="position: relative;">EMC Performing Arts Stuido</h2>
                    <p class="font-weight-light text-white" style="z-index: 100; position: relative; font-size: 1.2em !important;">
                      Creating digital content for a website and social media
                    </p>
                    <button class="mx-auto text-center d-block mb-5" style="position: relative; background: none; color: white; border: solid 2px #fbbc00; padding: 0.5em 1em;">View Work</button>
                  </router-link>
                  
                </div>
                <div class="row mb-5 pt-4 pb-5">
                  <a href="#" class="cta-button mx-auto" style="text-decoration: underline;">View all case studies</a>
                </div>



              </div>
            </div>

          
            

          </div>
        </template>
      
  </transition>


</template>

<style lang="scss" scoped>

p{
    font-size: 1.2em !important;
  }

  @media (min-width: 576px) {
   p{
    font-size: 1.5em !important;
  }
 }


  .link{
    color: white;
    &:hover{
      text-decoration: none;
    }
  }

  .ribbon{
    background-color: #a1d0c1;
    color: white;
  }

  .page-container{
    margin-top: 57vh;
  }

  .quote div {
    white-space: nowrap;
    width: 50%;
  }

  .quote {
    box-sizing: border-box;
    font-size: 2.7em;
    line-height: 1.5em;
  }


  // Medium devices (tablets, 768px and up)
  @media (max-width: 768px) { 
    .quote {
      font-size: 2em;
    }
 }

 @media (max-width: 576px) {
   .quote {
      font-size: 1.5em;
    }
 }

  .bg-txt{

    position: absolute;
    top: 21%;
    left: -5%;
    word-break: break-all;
    overflow-x: hidden;
    overflow-y: hidden;
    font-size: 8em;
    color: #1d1c1c;
    line-height: 1em;
    width: 118vw;
    display: inline;

  }

  del {
    text-decoration-color: #ffbd00;
  }

  ins {
    text-decoration: none;
    font-size: 1.1em;
    color: #ffbd00;
    position: absolute;
    font-weight: 500;
    -webkit-transform: rotate(-10deg);
    transform: rotate(-10deg);
    margin-left: 14em;
    margin-top: -3em;
    font-family: 'Permanent Marker', cursive;
    
  }

  .cover-photo{
    //background-position: top center;
    background-size: cover;
  }

</style>



<script>
  import {
    TweenLite,
    Power2,
    TweenMax,
    Power3,
    Power4
  } from "gsap";

  export default {
    name: "home",
    props:{
      errors: String
    },
    data() {
      return {
        animation: 'none',
        doneLoad: false
      }
    },
    transition: {
      enter(el, done) {
        let thisObj = this;
        if(this.$route.params.animation == 'fromHome'){
          TweenMax.to($('.fixed-wash'), 1, {
          delay: .5,
          css: {
            height: "1px",
            top: "67vh"
          },
          ease: Power4.easeInOut,
          onComplete: function () {
            $('.fixed-wash').addClass('d-none');
          }
        });
        TweenMax.from($('.cover-photo'), 1, {
          delay: .75,
          alpha: 0,
          scaleX: 1.1,
          scaleY: 1.1
        });

        TweenMax.from($('.ribbon'), .5, {
          alpha: 0,
          scaleY: 0
        });

        TweenMax.from($('#ribbon-title'), 1, {
          delay: 1.5,
          alpha: 0
        });
        }
      }
    },
    methods: {

    }
  };

</script>

