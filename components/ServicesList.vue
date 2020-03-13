<template>
    <div>
        <div class="row my-5">
          <h4 id="service-header" style="font-weight: bolder;" class="text-white pt-5">We create professional digital products,
            communications, and brands.</h4>
        </div>
        
        <div class="row pb-5 my-5">
          <div @click="toggleService('brand')" class="col-md-7 col-12 service-dropdown">
            <h3 style="font-weight: 400 !important;" class="text-white mx-auto font-weight-lighter">Brand Identity</h3>
            <svg style="max-width: 20px; color: rgb(255, 189, 0); position: absolute; top: 0px; left: 250px;" aria-hidden="true" focusable="false" data-prefix="fal" data-icon="caret-down" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 320 512" class="svg-inline--fa fa-caret-down fa-w-10 fa-2x"><path fill="currentColor" d="M287.968 160H32.038c-28.425 0-42.767 34.488-22.627 54.627l127.962 128c12.496 12.496 32.758 12.497 45.255 0l127.968-128C330.695 194.528 316.45 160 287.968 160zM160 320L32 192h256L160 320z" class=""></path></svg>
          </div>
          <div id="brand" class="col-md-8 col-12 pl-3 py-4 d-none">
            <h4 class="text-white font-weight-lighter">
              A brand today is all about how it makes your customers feel. It's not a logo or visual identity but rather a cohesive system that spans across all mediums and touchpoints. We're a branding firm offering a complete solution from naming and logo design to communications and style guides.
            </h4>
          </div>
          <div @click="toggleService('user')"  class="col-md-7 col-12 service-dropdown">
            <h3 style="font-weight: 400 !important;" class="text-white mx-auto font-weight-lighter">User Experience</h3>
            <svg style="max-width: 20px; color: rgb(255, 189, 0); position: absolute; top: 0px; left: 250px;" aria-hidden="true" focusable="false" data-prefix="fal" data-icon="caret-down" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 320 512" class="svg-inline--fa fa-caret-down fa-w-10 fa-2x"><path fill="currentColor" d="M287.968 160H32.038c-28.425 0-42.767 34.488-22.627 54.627l127.962 128c12.496 12.496 32.758 12.497 45.255 0l127.968-128C330.695 194.528 316.45 160 287.968 160zM160 320L32 192h256L160 320z" class=""></path></svg>
          </div>
          <div id="user" class="col-md-8 col-12 pl-3 py-4 d-none">
            <h4 class="text-white font-weight-lighter">
              A brand today is all about how it makes your customers feel. It's not a logo or visual identity but rather a cohesive system that spans across all mediums and touchpoints. We're a branding firm offering a complete solution from naming and logo design to communications and style guides.
            </h4>
          </div>
          <div @click="toggleService('dev')"  class="col-md-7 col-12 service-dropdown">
            <h3 style="font-weight: 400 !important;" class="text-white mx-auto font-weight-lighter">Development</h3>
            <svg style="max-width: 20px; color: rgb(255, 189, 0); position: absolute; top: 0px; left: 250px;" aria-hidden="true" focusable="false" data-prefix="fal" data-icon="caret-down" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 320 512" class="svg-inline--fa fa-caret-down fa-w-10 fa-2x"><path fill="currentColor" d="M287.968 160H32.038c-28.425 0-42.767 34.488-22.627 54.627l127.962 128c12.496 12.496 32.758 12.497 45.255 0l127.968-128C330.695 194.528 316.45 160 287.968 160zM160 320L32 192h256L160 320z" class=""></path></svg>
          </div>
          <div id="dev" class="col-md-8 col-12 pl-3 py-4 d-none">
            <h4 class="text-white font-weight-lighter">
              A brand today is all about how it makes your customers feel. It's not a logo or visual identity but rather a cohesive system that spans across all mediums and touchpoints. We're a branding firm offering a complete solution from naming and logo design to communications and style guides.
            </h4>
          </div>
          <div @click="toggleService('web')"  class="col-md-7 col-12 service-dropdown">
            <h3 style="font-weight: 400 !important;" class="text-white mx-auto font-weight-lighter">Websites</h3>
            <svg style="max-width: 20px; color: rgb(255, 189, 0); position: absolute; top: 0px; left: 250px;" aria-hidden="true" focusable="false" data-prefix="fal" data-icon="caret-down" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 320 512" class="svg-inline--fa fa-caret-down fa-w-10 fa-2x"><path fill="currentColor" d="M287.968 160H32.038c-28.425 0-42.767 34.488-22.627 54.627l127.962 128c12.496 12.496 32.758 12.497 45.255 0l127.968-128C330.695 194.528 316.45 160 287.968 160zM160 320L32 192h256L160 320z" class=""></path></svg>
          </div>
          <div id="web" class="col-md-8 col-12 pl-3 py-4 d-none">
            <h4 class="text-white font-weight-lighter">
              A brand today is all about how it makes your customers feel. It's not a logo or visual identity but rather a cohesive system that spans across all mediums and touchpoints. We're a branding firm offering a complete solution from naming and logo design to communications and style guides.
            </h4>
          </div>
        </div>
    </div>
</template>

<script>
import {
    TweenMax,
    Power3,
    Power4,
    TimelineLite
  } from "gsap";

import '../assets/vendor/SplitText.min.js';

export default {
    data() {
      return {
        animated: false,
        canAnimate: true,
      }
    },
    methods:{
        toggleService(clickedService){

            let thisObj = this;
            var clickedEl = "#" + clickedService;            
            if(thisObj.canAnimate){
                
                //$("#brand, #user, #dev, #web").addClass('d-none');
                if($(clickedEl).hasClass('d-none')){
                  $(clickedEl).removeClass('d-none');
                  var mySplitText = new SplitText($("#" + clickedService + ' h4')),
                  t2 = new TimelineLite();
                  mySplitText.split({type:"lines"}); 
                  t2.staggerFrom(mySplitText.lines, 0.25, { alpha: 0, y: 30, ease:Power4.easeOut}, 0.1, 0, allDone);

                  function allDone(){
                      mySplitText.revert();
                      thisObj.canAnimate = true;
                  }
                }else{
                  
                  var mySplitText = new SplitText($("#" + clickedService + ' h4')),
                  t2 = new TimelineLite();
                  mySplitText.split({type:"lines"}); 
                  t2.staggerTo(mySplitText.lines, 0.15, { alpha: 0, y: -30, ease:Power4.easeOut}, 0.1, 0, allDone);

                  function allDone(){
                      mySplitText.revert();
                      thisObj.canAnimate = true;
                      $(clickedEl).addClass('d-none');
                  }
                }
                
                
                thisObj.canAnimate = false;
                
            
            }
        }
    },
    mounted: function () {

      $.fn.isInViewport = function() {
        var elementTop = $(this).offset().top;
        var elementBottom = elementTop + $(this).outerHeight();

        var viewportTop = $(window).scrollTop();
        var viewportBottom = viewportTop + $(window).height();

        return elementBottom > viewportTop && elementTop < (viewportBottom + 100);
      };

      $(window).bind({
        resize: function () {
          checkViewStatus();
        },
        scroll: function () {
          checkViewStatus();
        }
      });

      
    let thisObj = this;

      function checkViewStatus() {
        if ($(thisObj.$el).isInViewport() && !thisObj.animated) {
            TweenMax.from($('#service-header'), .25, {delay: .5, alpha: 0, y: "+=30", ease:Power3.easeOut});
            TweenMax.staggerFrom($('.service-dropdown'), .25, {delay: .75, alpha: 0, y: "+=30", ease:Power3.easeOut}, .2);
            thisObj.animated = true;
        }
      }
      

    }
}
</script>