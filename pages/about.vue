

<template>



  <transition 
        v-on:enter="enter" 
        v-on:leave="leave"
        v-bind:css="false"
        appear
      >


        <template id="page">
          <div class="home page">

            



            <div id="home-content" >

              <div class="row mt-md-5 pt-5 mb-5 pb-lg-5">
                <div class="cover-photo" :style="{'background-image': 'url(' + require('@/assets/about/hero.jpg') + ')'}">
                  &nbsp;
                </div>
              </div>

              <div class="ribbon mx-0 row justify-content-between pl-4 px-md-5 no-gutters" style="background-color:#303f64;">
                <h2 id="ribbon-title" class="pt-1 my-3 mx-md-5" style="font-size: 1em; font-weight: 500;">Stephen Mark Toms <span style="color: #e2dede; font-weight: 300; font-size: 1em; margin-left: .5em;">Baltimore, Maryland</span> </h2>
                <h2 class="my-auto mx-sm-5" style="font-size: 1em; font-weight: 300; letter-spacing: .05em;"></h2>
              </div>

              <div class="page-container">
                <div class="row breakout mx-2 my-5 pb-5" >
								<div class="col-12 col-md-7">
									<h2 class="mt-5 mt-md-0 text-white text-left"><span style="font-weight: 200; font-size: 1.1em;">My Story </span></h2>
									<p class="text-left text-white" style="font-size: 1.1em;">
										 I was very young when my father died. But everyone tells me that his relationship with technology was effortless, he spoke gently and listened carefully, and he was never without a camera. It’s incredible that DNA can leave such a legacy. 
                     <br><br>
              			 This work for me is about the ability to synthesize my degree in Information Systems & Technology from Penn State with my desire to represent the individual, and the world around us, in a new and interesting way. The skills I acquired through my education and experiences allow me to create professional software, websites, videos, and photos. More importantly, I like people. I want to get to know you and to understand what’s important to you. Whether it’s creating an online presence for an artist, a piece of software, or building a brand for a local business, I believe in the work it takes to make every project perfect. 	
										
									</p>
									<br>
									<br>
									<h3 class="text-white text-left">
									- Stephen 
									</h3>
								</div>
								<div class="col-12 pt-5 pt-md-0 col-md-5 my-auto px-5 ">
									<img class="img-fluid mx-auto" :src="require('@/assets/about/dad.jpg')" >
								</div>	
							</div>
                <div class="row breakout d-none d-md-block" style="">
                  <div class="embed-responsive embed-responsive-16by9">
                    <video class="embed-responsive-item" autoplay muted loop> 
                      <source :src="require('@/assets/about/movie.webm')" type="video/webm">
                      <source :src="require('@/assets/about/movie.mp4')" type="video/mp4">
                    </video>
                  </div>
                </div>
                
                <!-- <div class="row breakout mt-5 pt-3 justify-content-center">
                  <div class="callout" style="background-position: 100% 27%;" :style="{'background-image': 'url(' + require('@/assets/case-studies/studio-eleven/hero-2.jpg') + ')'}">
                    &nbsp;
                  </div>
                </div> -->
                <div class="row py-5 px-md-5 breakout justify-content-center" style="background-color: white;">
                  <div class="px-0 px-md-5 mx-5 my-auto col-12" style="background-position: 100% 27%; " >
                    <p class="mx-5 px-5 text-left text-black" style="font-size: 1.5em; font-weight: 100;">
                        <span class="text-center text-md-left"> 
                          EXPERIENCE
                        </span>
                        <br>
												<div class="row px-0 mx-5 px-md-5 text-left">
													<div class="module-subtitle align-left gordita">
													<strong><b>Work:</b></strong> 
													<br>
													3 IT Technician
													<br>
													4 Years Freelance
													<br>
													1 Year Agency Life
													<br>
													<br>
													<strong><b>Degree: </b></strong> 
													<br>
													Pennsylvania State University BS in Information Systems and Technology
													<br>
													<br>
													<strong><b>Programming:</b></strong> 
													<br>
													JAVA, C++, C#, HTML5, XML, Node.js, Canvas, Bash, JavaScript, PHP, CSS3, Web Standards, SQL, MS Access, ActionScript 2.0, ActionScript 3.0, Adobe Flash CS4 - Creative Cloud 
													<br>
													<br>
													<strong><b>Libraries:</b></strong> 
													<br>
													GSAP/TweenMax, Barba.js, JQuery, PIXI.js, Three.js
													<br>
													<br>
													<strong><b>CMS:</b></strong> 
													<br>
													Craft, Wordpress, Expression Engine
													<br>
													<br>
													<strong><b>Databasing:</b></strong> 
													<br>
													SQL, phpMyAdmin, Seeding, Migrations
													<br>
													<br>
													<strong><b>Frameworks:</b></strong> 
													<br>
													Angluar/VueJS, React, Laravel, Bootstrap 4.0, Timber 
													<br>
													<br>
													<strong><b>IT/Deployment:</b></strong> 
													<br>
													IIS, DNS Configuration, Server Setup and Software Installation 
													<br>
													<br>
													<strong><b>Repository Management/Agile Workflow:</b></strong> 
													<br>
													Git, Bitbucket, Beanstalk
													<br>
													<br>
													<strong><b>Architectural Experience:</b></strong> 
													<br>
													Fullstack Software, Artificial Intelligence, Responsive Design, Object Oriented Programming, Encapsulation, Recursion, Model - View - Controller Design, Protype Creation, SEO, Usability Engineering, UML Diagramming, Database Diagrams, and In-Line Documentation. 
													<br>
													<br>
													<strong><b>Software:</b></strong> 
													<br>
													Adobe Creative Cloud, Microsoft 365, Sublime, VS Code, SQL Pro, WAMP, MAMP PRO
													</div>
												</div>
                      
                  </div>
                </div>
                <div class="row mt-5 pt-5 justify-content-center">
                  <!-- <div class="callout" style="background-position: bottom;" :style="{'background-image': 'url(' + require('@/assets/case-studies/jake-rivers/hero-6.jpg') + ')'}">
                    &nbsp;
                  </div> -->
                  <div class="embed-responsive embed-responsive-16by9">
                    <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/eNjVGVblZhI?rel=0" allowfullscreen></iframe>
                  </div>
                </div>
                
                <router-link class="no-dec" to="/works">
                  <div class="row mt-5 pt-5 breakout justify-content-center">
                    <div class="col mt-5" style="background-color: #252525;" >
                      <h4 class="no-dec my-auto " style="color: rgb(165, 165, 165); padding-top: 15%; padding-bottom: 15%;">View <span style="color: white;">works</span></h4>
                    </div>
                  </div>
                </router-link>

              </div>
            </div>

            <Footer></Footer>
           
            

          </div>
        </template>
      
  </transition>


</template>

<style lang="scss" scoped>

  @media(max-width: 500px){
    .page-container{
        margin-left: 0vw; 
        margin-right: 0vw; 
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
    background-position: top center;
    background-size: cover;
  }

</style>



<script>
/* eslint-disable */
import CaseStudy from '../components/CaseStudy.vue';
import Footer from '../components/Footer.vue';
export default {
  components: {
      Footer,
      CaseStudy,
  },
  name: "home",
  data() {
    return {
      animation: 'enter',
      doneLoad: false
    }
  },
  

  methods: {

    animateWash(){

          TweenMax.to($('.fixed-wash'), 1.3, {delay: .5, css:{height: "1px", top: "67vh"}, ease:Power4.easeInOut, onComplete: function(){
              $('.fixed-wash').addClass('d-none');
          }});
          TweenMax.from($('.cover-photo'), 1, {delay: .75, alpha: 0, scaleX: 1.1, scaleY: 1.1});

          TweenMax.from($('.ribbon'), .5, {alpha: 0, scaleY: 0});

          TweenMax.from($('#ribbon-title'), 1, {delay: 1.5, alpha: 0});

          

    },
    setNewAnimation: function (){

      this.animation = 'none';

      //alert("leaving " + this.animation);

      //this.$router.push('about');

    },


		enter: function enter(el, done) {

      


      $.fn.isInViewport = function() {
        var elementTop = $(this).offset().top;
        var elementBottom = elementTop + $(this).outerHeight();

        var viewportTop = $(window).scrollTop();
        var viewportBottom = viewportTop + $(window).height();

        return elementBottom > viewportTop && elementTop < (viewportBottom + 100);
      };

      


      console.log("entering " + this.animation);

        TweenMax.fromTo(el, 1, {
          autoAlpha: 0
          },
        {
				autoAlpha: 1,
				scale: 1,
				transformOrigin: '50% 50%',
				ease: Power4.easeOut,
        onComplete: done });
        

        this.animateWash();

        //end custom




		},
		leave: function leave(el, done) {
      
        //console.log("leaving " + this.animation);


        if(this.animation == 'none'){
          
          console.log("leaving NONE");
          TweenMax.fromTo(el, 1, {
				  autoAlpha: 0,
				  scale: 1.5 },
        {
          autoAlpha: 1,
          scale: 1,
          transformOrigin: '50% 50%',
          ease: Power4.easeOut,
          onComplete: done });

        }else{

          console.log("leaving Slide");
          
          
          TweenMax.fromTo(el, 1, {
				autoAlpha: 1 },
			{
				autoAlpha: 0,
				ease: Power4.easeOut,
				onComplete: done });



        }

        






        } 








    }
};


</script>
