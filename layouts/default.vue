<template>
  <div>
    <main role="main" class="main-content">
      <canvas id="noise" class="noise"></canvas>
    </main>
    <Navigation></Navigation>
    <canvas id="noise" class="noise"></canvas>
    <nuxt>
    </nuxt>
    <Footer id="footer"></Footer>
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
    mounted() {
      const noise = () => {
        let canvas, ctx;

        let wWidth, wHeight;

        let noiseData = [];
        let frame = 0;

        let loopTimeout;


        // Create Noise
        const createNoise = () => {
          const idata = ctx.createImageData(wWidth, wHeight);
          const buffer32 = new Uint32Array(idata.data.buffer);
          const len = buffer32.length;

          for (let i = 0; i < len; i++) {
            if (Math.random() < 0.5) {
              buffer32[i] = 0xff000000;
            }
          }

          noiseData.push(idata);
        };


        // Play Noise
        const paintNoise = () => {
          if (frame === 9) {
            frame = 0;
          } else {
            frame++;
          }

          ctx.putImageData(noiseData[frame], 0, 0);
        };


        // Loop
        const loop = () => {
          paintNoise(frame);

          loopTimeout = window.setTimeout(() => {
            window.requestAnimationFrame(loop);
          }, (1500 / 25));
        };


        // Setup
        const setup = () => {
          wWidth = window.innerWidth;
          wHeight = window.innerHeight;

          canvas.width = wWidth;
          canvas.height = wHeight;

          for (let i = 0; i < 10; i++) {
            createNoise();
          }

          loop();
        };


        // Reset
        let resizeThrottle;
        const reset = () => {
          window.addEventListener('resize', () => {
            window.clearTimeout(resizeThrottle);

            resizeThrottle = window.setTimeout(() => {
              window.clearTimeout(loopTimeout);
              setup();
            }, 200);
          }, false);
        };


        // Init
        const init = (() => {
          canvas = document.getElementById('noise');
          ctx = canvas.getContext('2d');

          setup();
        })();
      };

      noise();
    }
  }

</script>

<style lang="scss" scoped>
  .main-content {
    position: fixed;
    z-index: -1;
    top: 0;
    left: 0;
    width: 100vw;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-flow: column;

    height: 100vh;

    background: #171717;
    text-align: center;
  }

  .noise {
    z-index: 100;
    position: absolute;
    top: 0;
    left: 0;

    width: 100%;
    height: 100%;

    pointer-events: none;
    opacity: 1;
  }




</style>
