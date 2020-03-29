<template>



  <transition name="enter">


    <template id="page">
      <div class="home page">
        <div id="home-content">
          <div class="row mt-md-5 pt-5 mb-5 pb-lg-5">
            <div class="cover-photo"
              :style="{'background-image': 'url(' + require('@/assets/case-studies/studio-eleven/hero.jpg') + ')'}">
              &nbsp;
            </div>
          </div>
          <div class="ribbon mx-0 row justify-content-between pl-4 px-md-5 no-gutters">
            <h2 id="ribbon-title" class="pt-1 my-3 mx-md-5" style="font-size: 1em; font-weight: 500;">Studio Eleven
              <span style="color: #585858; font-weight: 300; font-size: 1em; margin-left: .5em;">Towson, Maryland</span>
            </h2>
            <h2 class="my-auto mx-sm-5" style="font-size: 1em; font-weight: 300; letter-spacing: .05em;">
              <!-- <a class="link d-none d-sm-block" href="https://studioeleven.us">visit site <i
                  class="fas fa-arrow-right"></i></a> -->
            </h2>
          </div>
          <div class="page-container">
            <div class="row my-5 py-5 justify-content-around">
              <div class="mx-auto col-12 col-lg-7 px-0 mt-2">

                <p class="newslab pt-lg-0 text-left" style="font-size: 1.5em; font-weight: 100;">
                  <span class="text-left" style="color: white; font-size: 1.1em; ">
                    QUICK WORDS
                  </span>
                  <br>
                  <span class="" style="color:white;">
                    Behind the scenes creative genius responsible for a Salon’s rebranding. Worked with models, and the
                    salon owners to establish their brand identity through capturing images, and social media.
                    <br>
                    <br>
                    Studio Eleven is a small upscale salon in the heart of Towson. Providing customized personal hair
                    services just for its clients in a relaxing environment. Studio Eleven specializes in Balayage (Hand
                    Painting), Custom Deep Conditioning Treatments, Color Corrections and Keratin Treatments.
                    <br>
                    <br>
                    The body of work encompassed creating a brand, website, photography, a promotional video, and
                    tracking website analytics.
                  </span>
                </p>
              </div>
              <div class="pt-5 col-2 px-0  mx-5 d-none d-lg-block">
                <p class="pt-5 pt-lg-0 text-left" style="font-size: 1em; font-weight: 100;">
                  <span style="color: white; font-size: .9em; font-weight: 500;">
                    client:
                  </span>
                  <br>
                  <span class="newslab" style="color:white;">
                    Studio Eleven<br>
                  </span>
                  <p class="pt-5 pt-lg-0 text-left" style="font-size: 1em; font-weight: 100;">
                    <span style="color: white; font-size: .9em; font-weight: 500;">
                      output:
                    </span>
                    <br>
                    <span class="newslab" style="color:white;">
                      Branding<br>
                      Website<br>
                      Photography<br>
                      Videography
                    </span>
                  </p>
              </div>
            </div>
            <div class="row breakout d-none d-md-block" style="">
              <div class="embed-responsive embed-responsive-16by9">
                <video class="embed-responsive-item" autoplay muted loop>
                  <source :src="require('@/assets/case-studies/studio-eleven/movie.webm')" type="video/webm">
                  <source :src="require('@/assets/case-studies/studio-eleven/movie.mp4')" type="video/mp4">
                </video>
              </div>
            </div>
            <div class="row d-none d-md-block mt-5 p-3 justify-content-center"
              style="background-color: white; border: solid 10px #ccc8c8;">
              <div class="px-5 my-auto col-12" style="background-position: 100% 27%; ">
                <img style="width: 100%; height: auto;"
                  :src="require('@/assets/case-studies/studio-eleven/website-1.png')">
              </div>
            </div>
            <div class="row d-none d-md-block mt-5 p-3 justify-content-center"
              style="background-color: white; border: solid 10px #ccc8c8;">
              <div class="px-5 my-auto col-12" style="background-position: 100% 27%; ">
                <img style="width: 100%; height: auto;"
                  :src="require('@/assets/case-studies/studio-eleven/website-2.png')">
              </div>
            </div>
            <div class="row d-none d-md-block mt-5 p-3 justify-content-center"
              style="background-color: white; border: solid 10px #ccc8c8;">
              <div class="px-5 my-auto col-12" style="background-position: 100% 27%; ">
                <img style="width: 100%; height: auto;"
                  :src="require('@/assets/case-studies/studio-eleven/website-3.png')">
              </div>
            </div>
            <div class="row d-none d-md-block mt-5 mb-5 p-3 justify-content-center"
              style="background-color: white; border: solid 10px #ccc8c8;">
              <div class="px-5 my-auto col-12" style="background-position: 100% 27%; ">
                <img style="width: 100%; height: auto;"
                  :src="require('@/assets/case-studies/studio-eleven/website-4.png')">
              </div>
            </div>
            <div class="row breakout pt-5 mt-5 p-3 py-5 justify-content-center" style="background-color: #f0f0f0;">
              <div class="px-5 my-5 my-md-auto col-12 col-md-3" style="background-position: 100% 27%; ">
                <img style="width: 100%; height: auto;"
                  :src="require('@/assets/case-studies/studio-eleven/mobile/1.jpg')">
              </div>
              <div class="px-5 my-5 my-md-auto col-12 col-md-3" style="background-position: 100% 27%; ">
                <img style="width: 100%; height: auto;"
                  :src="require('@/assets/case-studies/studio-eleven/mobile/2.jpg')">
              </div>
              <div class="px-5 my-5 my-md-auto col-12 col-md-3" style="background-position: 100% 27%; ">
                <img style="width: 100%; height: auto;"
                  :src="require('@/assets/case-studies/studio-eleven/mobile/3.jpg')">
              </div>
              <div class="px-5 my-5 my-md-auto col-12 col-md-3" style="background-position: 100% 27%; ">
                <img style="width: 100%; height: auto;"
                  :src="require('@/assets/case-studies/studio-eleven/mobile/4.jpg')">
              </div>
            </div>
            <div class="row py-5 px-md-5 breakout justify-content-center" style="background-color: white;">
              <div class="px-5 my-auto col-12 col-lg-6 col-xl-4" style="background-position: 100% 27%; ">
                <p class="px-lg-5 pt-lg-0 text-left text-black" style="font-size: 1.5em; font-weight: 100;">
                  <span class="text-left newslab" style="font-size: 1.1em;">
                    ESTABLISHING A BRAND
                  </span>
                  <br>
                  <span class="">
                    Working with the Studio Eleven logo, a bright color pallet was established. Pastels were chosen to
                    keep a light and feminine design.
                  </span>
                </p>
              </div>
              <div class="px-5 my-auto col-12 col-lg-6 col-xl-4 d-flex mx-auto" style="background-position: 100% 27%; ">
                <img style="max-width: 100%;" :src="require('@/assets/case-studies/studio-eleven/logo.png')">
              </div>
              <div class="col-12 mt-5 text-center">
                <h3>COLOR</h3>
              </div>
              <div class="col-12 mt-4">
                <div class="row mb-5 justify-content-center">
                  <div class="col-3 color-pallet" style="background-color: #e7efec;">
                    &nbsp;
                  </div>
                  <div class="col-3 color-pallet" style="background-color: #f6e2dd;">
                    &nbsp;
                  </div>
                  <div class="col-3 color-pallet" style="background-color: #d9eaee;">
                    &nbsp;
                  </div>
                  <div class="col-3 color-pallet" style="background-color: #bab8c6;">
                    &nbsp;
                  </div>
                </div>
              </div>
            </div>
            <div class="row mt-5 pt-5 justify-content-center">
              <div class="callout" style="background-position: 100% 27%;"
                :style="{'background-image': 'url(' + require('@/assets/case-studies/studio-eleven/hero-6.jpg') + ')'}">
                &nbsp;
              </div>
            </div>
            <div class="row my-5 pt-5 justify-content-around">
              <div class="mx-auto col-12 col-lg-10 px-0 mt-2">
                <p class="pt-5 pt-lg-0 text-left" style="font-size: 1.5em; font-weight: 100;">
                  <span class="newslab text-left" style="color: white; font-size: 1.1em;">
                    TELLING A STORY
                  </span>
                  <br>
                  <span class="" style="color:white;">
                    Part of the branding experience was establishing a modern look for the company. With this goal in
                    mind, while capturing photography and videography, this was created by posing the models
                    organically.
                  </span>
                </p>
              </div>
            </div>
            <div class="row mt-5 pt-3 justify-content-around">
              <div class="col-12 col-md-5 ">
                <div class="callout" style="border: solid 14px #e4efec; background-position: 56% 46%;"
                  :style="{'background-image': 'url(' + require('@/assets/case-studies/studio-eleven/hero-3.jpg') + ')'}">
                  &nbsp;
                </div>
              </div>
              <div class="mt-5 mt-md-0 col-12 col-md-5 ">
                <div class="callout" style="border: solid 14px #e4efec; background-position: 100% 27%;"
                  :style="{'background-image': 'url(' + require('@/assets/case-studies/studio-eleven/hero-4.jpg') + ')'}">
                  &nbsp;
                </div>
              </div>
            </div>
            <div class="row mt-5 pt-5 breakout justify-content-center">
              <div class="callout" style="background-position: 75% 27%;"
                :style="{'background-image': 'url(' + require('@/assets/case-studies/studio-eleven/hero-2.jpg') + ')'}">
                &nbsp;
              </div>
            </div>
            <div class="row my-5 pt-5 justify-content-around">
              <div class="mx-auto col-12 col-lg-10 px-0 mt-2">
                <p class="pt-5 pt-lg-0 text-left" style="font-size: 1.5em; font-weight: 100;">
                  <span class="text-left newslab" style="color: white; font-size: 1.1em;">
                    FINAL RESULTS
                  </span>
                  <br>
                  <span class="" style="color:white;">
                    After establishing brand, creating fresh content, a simple site was designed. The provided logo was
                    broken apart to convey the brand through the website as a whole instead of staying locked in the
                    logo area. Every color used was of a light pastel to keep a soft feel. While laying in content and
                    writing copy the grid layout was broken to emphasize importance to certain sections.
                    <br><br>
                    Using modern web standards the responsive design and pixel tracking was implemented to enhance
                    compatibility, measure the success and user behavior.
                  </span>
                </p>
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
            <!-- <router-link class="no-dec" to="/callie-tomblin">
              <div class="row mt-5 pt-5 breakout justify-content-center">
                <div class="col mt-5" style="background-color: #252525;">
                  <h4 class="no-dec my-auto " style="color: rgb(165, 165, 165); padding-top: 15%; padding-bottom: 15%;">
                    Next Project: <br><span style="color: white;">Callie Tomblin</span></h4>
                </div>
              </div>
            </router-link> -->
          </div>
        </div>

      </div>
    </template>

  </transition>


</template>

<style lang="scss" scoped>
  p {
    font-size: 1.2em !important;
  }

  @media (min-width: 576px) {
    p {
      font-size: 1.5em !important;
    }
  }


  .link {
    color: white;

    &:hover {
      text-decoration: none;
    }
  }

  .ribbon {
    background-color: #a1d0c1;
    color: white;
  }

  .page-container {
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

  .bg-txt {

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
