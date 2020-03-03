
<template id="page">
          <div class="home page">

            
        
            <Navigation></Navigation>


            <div id="home-content" class="page-container">

              <div class="row mt-md-5 pt-5 mb-5 pb-lg-5">
                <div class="col-12 col-lg-12 px-0 mt-2">
                  <h1 class="quote text-left text-white mb-0 mt-lg-3">A multimodal designer based in Baltimore, MD. Creating brand identities, applications, websites and visual experiences to help organizations innovate their business.</h1>
                </div>
              </div>

              <div class="row mx-0 mt-md-5">
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

          

            <Footer id="footer" ></Footer>
           
            

          </div>
</template>
      


<style lang="scss" scoped>

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
import Navigation from '../components/Navigation.vue';
import Footer from '../components/Footer.vue';
import {TweenMax, Power4, TimelineLite} from "gsap";
import '../assets/vendor/SplitText.min.js';

export default {
  components: {
      Navigation,
      Footer,
      CaseStudy,
  },
  name: "home",
  data() {
    return {
      animation: 'enter',
      doneLoad: false,
      nextPage: 'studio-eleven',
    }
  }
  
};


</script>
