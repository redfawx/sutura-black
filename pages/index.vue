
<template id="page">
    <transition name="enter">
          <div class="home page">

            
        
           


            <div id="home-content" class="page-container">

              

            <div class="d-flex" style=" min-height: 80vh;">
              <div class="my-auto">
                  <h1 class="quote text-left text-white mb-0 mt-lg-3">
                    <span style="font-weight: 300; ">SUTURA</span> is a web design and<br class="d-none d-md-block"> branding agency in Baltimore.
                  </h1>
              </div>
              <div style="position: absolute; max-width: 1002px; width: 67vw; right: 0; top: 50%; transform: translateY(-50%);">
                <div style="background-color: #181818c4; width: 100%; height: 100%; position: absolute;"></div>
                <video playsinline="" autoplay="autoplay" loop="loop" muted="muted" preload="auto" class="my-auto mx-auto w-100"><source :src="require('@/assets/home/promo.mp4')" type="video/mp4">
                </video>
              </div>
            </div>


            

              <div class="row mx-0 mt-md-5 pt-md-5">
                <div class="col-12 px-0  mx-0">

                  <div class="row justify-content-between">

                    <div class="case-study  px-0 col-md-5 col-12 mx-0 text-left"
                    >

                      <CaseStudy
                          
                          ref="case1"
                          name="Studio Eleven" 
                          id="studio-eleven" 
                          thumbnail="studio-eleven" 
                          title="Studio Eleven Hair Salon"
                          disc="Creating a brand identity and website refresh for an upcoming hair salon"
                          color="#a1d0c1"
                      ></CaseStudy>
                    </div>

                    <div class="case-study  px-0 col-md-6 col-12 mx-0 mt-2 text-left my-md-auto">
                      <CaseStudy class="mt-6 my-md-auto"
                          ref="case2"
                          name="Callie Tomblin" 
                          id="callie-tomblin" 
                          thumbnail="callie-tomblin" 
                          title="Callie Tomblin"
                          disc="Establishing a brand identity for a musician"
                          color="#D1B160"
                      ></CaseStudy>
                    </div>

                  </div>

                </div>
              </div>

              <div class="row mx-0 mt-md-5">
                <div class="col-12 px-0 mt-lg-5 mx-0">

                  <div class="row mt-md-10 justify-content-end">

                     <div class="case-study  px-0 col-md-10 col-12 mx-0 mt-2 text-left">
                        <CaseStudy class="my-lg-5 "
                            ref="case3"
                            name="Jake Matthew Rivers" 
                            id="jake-rivers" 
                            thumbnail="jake-rivers" 
                            title="Jake Matthew Rivers"
                            disc="Establishing a brand identity and promotional video for a musician"
                            color="#b73a40"
                            
                        ></CaseStudy>
                     </div>


                  </div>

                </div>
              </div>


              <div class="row mx-0 mt-md-5">
                <div class="col-12 px-0 mt-lg-5 mx-0">

                  <div class="row mt-md-10 justify-content-between">

                     <div class="case-study  px-0 col-md-5 my-auto col-12 mx-0 mt-2 text-left">
                        <CaseStudy class="my-lg-5"
                            name="Joppa View Elementary School" 
                            thumbnail="jve" 
                            id="joppa-view" 
                            title="Joppa View Elementary School"
                            disc="Creating a organic video for social media awareness"
                            color="#8DD9FD"
                        ></CaseStudy>
                     </div>

                     <div class="case-study  px-0 col-md-6 col-12 mx-0 mt-2 text-left">
                        <CaseStudy class="my-lg-5"
                            name="EMC Performing Arts" 
                            thumbnail="emc" 
                            id="emc" 
                            title="EMC Performing Arts"
                            disc="Creating digital content for a website and social media"
                            color="#BBC5A1"
                        ></CaseStudy>
                     </div>


                  </div>

                </div>
              </div>



            </div>

          

            
           
            

          </div>
    </transition>
</template>
      


<style lang="scss" scoped>

  .quote div {
    white-space: wrap;
    width: 50%;
  }

  .quote:first-child::nth-line(-1+2) {
    font-variant-caps: small-caps;
    color: red !important;
  }

  .quote {
    box-sizing: border-box;
    line-height: 1.5em;
    font-weight: 700;
    font-size: 4em;
    z-index: 100;
    position: relative
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
    // width: 118vw;
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

import CaseStudy from '../components/CaseStudy.vue';
import PromoVideo from '../components/PromoVideo.vue';

import {TweenMax, Power4, TimelineLite} from "gsap";
import '../assets/vendor/SplitText.min.js';

export default {
  components: {
      CaseStudy,
      PromoVideo
  },
  name: "home",
  data() {
    return {
      
    }
  },
  transition: {
    name: 'enter',
    enter(el, done){
      // console.log('enter');
      // var mySplitText = new SplitText($(".quote")),
      // t2 = new TimelineLite();

      // mySplitText.split({type:"lines"}); 
      // t2.staggerFrom(mySplitText.lines, 0.75, {delay: .5, opacity:0, y: 100, ease:Power4.easeOut}, 0.2, 0, allDone);

      // function allDone(){
      //   mySplitText.revert();
      // }

    },
    leave(el, done){
    
          console.log("leaving NONE");
          TweenMax.to(el, .5, { opacity: 0, ease: Power4.easeOut, onComplete: done});
    }
  },
  
  methods:{
    
  }
  
};


</script>
