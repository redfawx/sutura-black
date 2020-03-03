<template>

    
      <div >

          <!-- <div class="wash"> -->
          
          <div class="wash" style="background-color: #292929;">
            

            <img class="img-fluid"  v-bind:src="imgSrc" />

            <div class="row mt-5 scroller-row">
              <div class="scroller mt-5">
                    <div class="lines">
                        <div class="line">
                          <span>{{ name }}</span>
                          <span>{{ name }}</span>
                          <span>{{ name }}</span>
                          <span>{{ name }}</span>
                          <span>{{ name }}</span>
                        </div>
                        <div class="line">
                            <span>{{ name }}</span>
                            <span>{{ name }}</span>
                            <span>{{ name }}</span>
                            <span>{{ name }}</span>
                            <span>{{ name }}</span>
                        </div>
                    </div>
                </div>
            </div>
            <!-- <div class="hover" style="background-color:#171717; width: 100%; height: 100%; position: absolute; top: 0; "></div> -->
          </div>

          
          
          <h4 class="header text-white mt-3" ><span class="title-disc">{{ title }}</span></h4>
          <p class="header mt-1 pr-4" >{{ disc }}</p>

          
        
          

      </div>
      


</template>

<script>

import {TweenLite, Power2} from "gsap";

export default {
  data(){
    return{
      animated: false,
      imgSrc: require('@/assets/' + this.thumbnail + '.jpg'),
      link: "",
      doneLoad: false,
    }
  },
  props: {
    name: String,
    thumbnail: String,
    title: String,
    disc: String,
    color: String,
    id: String,
  }
  
};



</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" >


  /* Page content */
  .content {
    padding: 16px;
  }

  /* The sticky class is added to the header with JS when it reaches its scroll position */
  .sticky {
    position: fixed;
    top: 0;
    width: 100%
  }

  /* Add some top padding to the page content to prevent sudden quick movement (as the header gets a new position at the top of the page (position:fixed and top:0) */
  .sticky + .content {
    padding-top: 102px;
  }

  .hover{

    cursor: pointer;

  }

  .case-img{

    //border-bottom: solid 4px #ffc400;
    cursor: pointer;
    transition: all 0.5s ease;

  }
  
  .title-disc{

    text-decoration: none;
    //border-bottom: 3px solid #ffaf1e;
    padding-bottom: 0px;

  }

  .scroller-row{

    position: absolute;
    bottom: 28%;
    opacity: 1;
    transition: all 0.5s ease;

  }


  .scroller {
        overflow: hidden;
        width: 100%;
        //opacity: 0;
        transition: all 0.5s ease;
    }

    .lines {
        display: flex;
        flex-direction: row;
        flex-wrap: nowrap;  
        font-size: 7em;
        font-weight: 800;
        color: white;
        transition: all 0.5s ease;
    }

    .line {
        animation: scrollerAnime 30s linear infinite;
        display: flex;
        flex-direction: row;
        flex-wrap: nowrap;
        justify-content: flex-start;
        align-content: flex-start;
        align-items: flex-start;
        white-space: nowrap;
        // transition: all 0.5s ease;
    }

    .line span {
        padding-right: 0.5em;
    }
    
    .line span:after {
        content: ' ';
        margin-left: 0.5em;
    }

    @keyframes scrollerAnime {
        0% {
            transform: translate3d(0, 0, 0);
        }
        100% {
            transform: translate3d(-100%, 0, 0);
        }
    }



  h2{

    font-size: 3em;

  }

  .header{

    font-size: 1em;

  }

  p{

    font-family: sailec-thin;
    font-size: .9em;
    color: #a9a9a9;

  }

  .wash{

    // background-color: red;
    z-index: 2;

  }

  img{

    // opacity: .6;
    //transition: all 0.5s ease;
    transform: scaleX(1.01);

  }

  .disc{

    font-size: 8em;
    font-weight: 800;
    color: white;
    position: absolute;
    top: 30%;
    background-color: red;


  }

  .disc2{

    position: absolute;
    top: 50%;

  }


.marquee {
  margin: 0 auto;
  white-space: nowrap;
  overflow: hidden;
  position: absolute;
}

.marquee span {
  display: inline-block;
  padding-left: 80%;
  animation: marquee 6s linear infinite;
}

.marquee2 span {
  animation-delay: 3s;
}

#mar1{

    color: white;
    font-size: 5em;
    font-weight: 800;

}

#mar2{

    color: white;
    font-size: 5em;
    font-weight: 800;

}

@keyframes marquee {
  0% {
    transform: translate(0, 0);
  }
  100% {
    transform: translate(-100%, 0);
  }
}

  



</style>
