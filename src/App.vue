<template>
  <div id="app" style="background-color: #111827;
">
    <barra-vue/>

    <div class="m-4">
       <div class="row">
       <div class="col-md-6">
        <ProfileVue/>
         <about-vue/>
       </div>
       <div class="col-md-6">
         <div class="row">
           <TecnologiesVue/>

           <div class="col-md-6">
           <LenguagesVue/>
           </div>
           <div class="col-md-6">
             <languagesRatingVue/>
           </div>
         </div>
       </div>
           <div class="col-md-12">
            <projects-vue/>
         </div>
       </div>
    </div>

  <FooterVue/>

  </div>
</template>

<script>
import BarraVue from './components/barraVue.vue'
import languagesRatingVue from './components/lenguagesRatingVue'
import ProfileVue from './components/profileVue.vue'
import LenguagesVue from './components/lenguagesVue.vue'
import TecnologiesVue from './components/tecnologiesVue.vue'
import ProjectsVue from './components/projectsVue.vue'
import AboutVue from './components/aboutVue.vue'
import FooterVue from './components/footerVue.vue'

export default {
  name: 'App',
  components: {
    BarraVue,
    ProfileVue,
    LenguagesVue,
    TecnologiesVue,
    languagesRatingVue,
    ProjectsVue,
    AboutVue,
    FooterVue
}
}
</script>
<style>
body {
  background-color: #111827;
  background-size: cover; /* for IE9+, Safari 4.1+, Chrome 3.0+, Firefox 3.6+ */
  -webkit-background-size: cover; /* for Safari 3.0 - 4.0 , Chrome 1.0 - 3.0 */
  -moz-background-size: cover; /* optional for Firefox 3.6 */
  -o-background-size: cover; /* for Opera 9.5 */
  margin: 0; /* to remove the default white margin of body */
  padding: 0; /* to remove the default white margin of body */
  overflow: auto;
}
</style>
