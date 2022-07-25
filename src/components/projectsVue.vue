<template>
     <b-container class="mt-5" >
    <b-badge class="w-100 text-white font-weight-bolder mx-auto p-1" variant="dark">{{$t('messageProjects')}}</b-badge>
    <b-carousel
        id="carousel"
        style="text-shadow: 0px 0px 5px black;"
        v-model="open_slide"
        :interval="0"
        controls
        indicators
    >
      <a :href="slides[open_slide].link">
         <b-carousel-slide
         v-for="(slide, index) in slides"
        :key="index"
        :caption="slide.caption"
        :img-src="slide.src"
        :id="slide.link"
        class="vtam"
        text="click to open"
     >
     </b-carousel-slide>
      </a>
    </b-carousel>
    </b-container>
</template>

<script>
export default {
    name: 'projectsVue',
    data() {
        return {
            slides: [
              {caption: "RestMethodsRefit Nuget package", src: require("../assets/projects/refitRestMethods.png"), link: "https://github.com/FabriGinseng/RestMethodsRefit"},
              {caption: "HCM System", src: require("../assets/projects/conceptMapEntropy.png"), link: "https://github.com/FabriGinseng/EntropyProject"},
              {caption: "Campania in salute", src: require("../assets/projects/cis.png"), link: "https://play.google.com/store/apps/details?id=it.almaviva.soresa.campaniainsalute&gl=IT"},
              {caption: "Quick Queue System", src: require("../assets/projects/quick.png"), link: "https://www.ak12srl.it/app7.html"},
            ],
            open_slide: 0
        }
    }

}
</script>

<style>
.vtam {
   height:40vh;
   background: #292b2c;
 }
</style>
