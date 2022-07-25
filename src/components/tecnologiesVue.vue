<template>
  <b-container>
    <b-card class="container shadow-lg rounded mt-5" style="background-color: #1f2937" text-variant="light">
      <span class="text-light font-weight-bold">{{$t('messageTechnology')}}</span> <br />
      <span class="text-secondary">({{$t('subtitleTechnology')}})</span>

      <hr />

      <div class="img-content">
        <i
          class="_icons m-2"
          v-for="(svg, index) in items"
          :id="'icon:' + index"
          :key="index"
          v-on:mouseover="colorful('icon:' + index)"
          v-on:mouseleave="colorless('icon:' + index)"
          v-on:click="colorful('icon:' + index)"
          :class="svg.data"
        ></i>
      </div>
    </b-card>
  </b-container>
</template>

<script>
export default {
  name: "tecnologiesVue",
  data() {
    return {
      items: [
        { data: "devicon-csharp-plain" },
        { data: "devicon-xamarin-plain" },
        { data: "devicon-visualstudio-plain" },
        { data: "devicon-javascript-plain" },
        { data: "devicon-typescript-plain" },
        { data: "devicon-vuejs-plain" },
        { data: "devicon-nodejs-plain" },
        { data: "devicon-electron-original"},
        { data: "devicon-intellij-plain"},
        { data: "devicon-phpstorm-plain"},
        { data: "devicon-java-plain" },
        { data: "devicon-dotnetcore-plain" },
        { data: "devicon-cplusplus-plain" },
        { data: "devicon-bootstrap-plain" },
        { data: "devicon-mysql-plain" },
        { data: "devicon-mongodb-plain" },
        { data: "devicon-trello-plain" },
        { data: "devicon-git-plain" },
        { data: "devicon-html5-plain" },
        { data: "devicon-css3-plain" },
        { data: "devicon-sqlite-plain" },
        { data: "devicon-linux-plain" },
        { data: "devicon-raspberrypi-line" },
        { data: "devicon-arduino-plain" },
        { data: "devicon-androidstudio-plain" },
        { data: "devicon-android-plain" },
      ],
    };
  },
  methods: {
    colorful(id) {
      document.getElementById(id).classList.add("colored");
    },
    colorless(id) {
      document.getElementById(id).classList.remove("colored");
    },
  },
};
</script>

<style scoped>
._icons {
  font-size: 40px;
  transition: 500ms;
}
._icons:hover {
  font-size: 60px;
  transition: 500ms;
}
</style>
