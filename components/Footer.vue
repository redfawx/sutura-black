<template>

    <div class="row mt-5">
        <div class="row mt-5">
            <div class="row mt-5">
                <div class="scroller mt-5">
                    <router-link class="no-dec" to="/about">
                        <a href="#" class="marquee-link">    
                            <div class="lines">
                                <div class="line">
                                    <span>About</span>
                                    <span>About</span>
                                    <span>About</span>
                                    <span>About</span>
                                    </div>
                                    <div class="line">
                                    <span>About</span>
                                    <span>About</span>
                                    <span>About</span>
                                    <span>About</span>
                                </div>
                            </div>
                        </a>
                    </router-link>
                </div>
            </div>

            <div class="row py-3 bg-black" >
                <div class="scroller-2">
                    <router-link class="no-dec" to="/contact">
                    <div class="lines-2">
                        <div class="line-2">
                            <span>Get in Touch</span>
                            <span>Get in Touch</span>
                            <span>Get in Touch</span>
                        </div>
                        <div class="line-2">
                            <span>Get in Touch</span>
                            <span>Get in Touch</span>
                            <span>Get in Touch</span>
                        </div>
                    </div>
                    </router-link>
                </div>
            </div>
        </div>
        <div class="row mb-0 mx-auto breadcrumb bg-black mr-5 pr-md-5">
            <div class="col-12 col-lg-6 ml-lg-1 pl-auto">
                <a href="/about">
                    <p class=" text-lg-left" style="color: #444137; text-decoration: none;">
                        SMT Designs 2019 designed and developed by Stephen Mark Toms
                    </p>
                </a>
            </div>
            
            <div class="col-12 col-lg-5 pr-0" >
                
                    <p class="d-none mr-5 pr-md-5 text-white text-lg-right">
                        <a href="#" class="text-white px-1 px-md-3">
                            LinkedIn
                        </a>
                        <a href="#" class="text-white px-1 px-md-3">
                            Facebook
                        </a>
                        <a href="#" class="text-white px-1 px-md-3">
                            Instagram
                        </a>
                        <a href="#" class="text-white px-1 px-md-3">
                            GitHub
                        </a>
                    </p>
                
                
            </div>
        </div>
    </div>
    


</template>

<script>
export default {
  name: "Footer",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>

    .marquee-link{

        text-decoration: none;

        &:hover{

            color: white !important;

        }

    }

    .breadcrumb{

        width: 100vw;

    }

    .scroller {
        overflow: hidden;
        width: 100%;
        
    }

    

    .lines {
        display: flex;
        flex-direction: row;
        flex-wrap: nowrap;  
        font-size: 7em;
        font-weight: 800;
        color: #202020;
        transition: all 0.5s ease;

        &:hover{

            color: white !important;

        }

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

    .scroller-2 {
        overflow: hidden;
        width: 100%;
    }

    .lines-2 {
        display: flex;
        flex-direction: row;
        flex-wrap: nowrap;  
        font-size: 7em;
        font-weight: 800;
        color: #202020;

        transition: all 0.5s ease;

        &:hover{

            color: white !important;

        }

    }

    .line-2 {
        animation: scrollerAnime2 30s linear infinite;
        display: flex;
        flex-direction: row;
        flex-wrap: nowrap;
        justify-content: flex-start;
        align-content: flex-start;
        align-items: flex-start;
        white-space: nowrap;

    }

    .line-2 span {
        padding-right: 0.5em;
    }
    
    .line-2 span:after {
        content: ' ';
        margin-left: 0.5em;
    }

    @keyframes scrollerAnime2 {
        0% {
            transform: translate3d(-100%, 0, 0);
        }
        100% {
            transform: translate3d(0, 0, 0);
        }
    }

    @media (max-width: 576px) {
        .lines{
            font-size: 4em;
        }
        .lines-2{
            font-size: 4em;
        }
    }

    

</style>
