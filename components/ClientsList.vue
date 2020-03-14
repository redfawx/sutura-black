<template>
  <div>
    <div class="row my-5">
      <h4 id="clients-header" style="font-weight: bolder;" class="text-white mx-auto pt-5">Featured Engagements</h4>
    </div>

    <div id="clients-row" class="row justify-content-center mt-5 ">
      <div class="col-4 my-auto">
        <div class="img-holder d-flex my-auto mb-5">
          <img class="d-flex mx-auto my-auto " :src="require('@/assets/home/logos/evangelin.png')" />
        </div>
        <p class="mt-4">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Sapiente excepturi consequatur nihil soluta
          repudiandae vitae, nesciunt a doloribus repellat ut enim corporis. Quisquam ratione harum, officiis assumenda
          hic praesentium labore.
        </p>
      </div>
      <div class="col-4 my-auto">
        <div class="img-holder d-flex my-auto mb-5">
          <!-- <img class="d-flex mx-auto my-auto " :src="require('@/assets/home/logos/evangelin.png')" /> -->
          <img style="max-width: 180px;" class="d-flex mx-auto my-auto  img-fluid" :src="require('@/assets/home/logos/studio-eleven.png')" />
        </div>
        <p class="mt-4">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Sapiente excepturi consequatur nihil soluta
          repudiandae vitae, nesciunt a doloribus repellat ut enim corporis. Quisquam ratione harum, officiis assumenda
          hic praesentium labore.
        </p>
      </div>
      <div class="col-4 my-auto">
        <div class="img-holder d-flex my-auto mb-5">
          <img class="d-flex mx-auto my-auto " :src="require('@/assets/home/logos/emc.png')" />
        </div>
        <p class="mt-4">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Sapiente excepturi consequatur nihil soluta
          repudiandae vitae, nesciunt a doloribus repellat ut enim corporis. Quisquam ratione harum, officiis assumenda
          hic praesentium labore.
        </p>
      </div>
    </div>
    <div class="row my-5 py-5">
      <a href="#" id="clients-button" class="cta-button mx-auto" style="text-decoration: underline;">View all clients</a>
    </div>
  </div>
</template>

<script>
import {
    TweenMax,
    Power4
  } from "gsap";
export default {
    data() {
      return {
        animated: false,
        canAnimate: true,
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
            console.log('inView');
            TweenMax.from($('#clients-header'), .25, {delay: .75, alpha: 0, ease:Power4.easeOut});
            TweenMax.staggerFrom($('#clients-row .col-4'), .25, {delay: 1, alpha: 0, y: "+=30", ease:Power4.easeOut}, .2);
            thisObj.animated = true;
        }
      }
    }
}
</script>