<template>
  <b-navbar toggleable="lg" class="navbar-horizontal shadow-lg">
    <b-navbar-brand>
      <b-icon icon="person-circle" variant="dark"></b-icon>
      <span class="font-weight-bold mt-auto ml-2"> Antonio Fabrizio Fiume</span>
    </b-navbar-brand>

    <b-navbar-nav>
      <b-nav-item href="#" class="mt-auto ml-auto">
        <b-badge variant="white">
          <b-icon variant="secondary" icon="code-slash"></b-icon>
          <span class="text-secondary">Software developer </span>
        </b-badge>
      </b-nav-item>
      <b-nav-item
        href="https://goo.gl/maps/UjyFKjD347AcvrDk6"
        class="mt-auto ml-auto">
        <b-badge variant="white">
          <b-icon
              variant="secondary"
              scale="0.9"
              icon="geo-alt"
          ></b-icon>
          <span class="text-secondary">Italy. Naples </span>
    </b-badge
      ></b-nav-item>
    </b-navbar-nav>

    <b-navbar-nav class="ml-auto display-inline">
      <b-nav-item :href="github"
        ><b-icon icon="github" variant="dark"></b-icon
      ></b-nav-item>
      <b-nav-item :href="mail"
        ><b-icon icon="envelope-fill" variant="dark"></b-icon
      ></b-nav-item>
      <b-nav-item :href="linkedin"
        ><b-icon icon="linkedin" variant="dark"></b-icon
      ></b-nav-item>
    </b-navbar-nav>
  </b-navbar>
</template>

<script>
export default {
  name: "barraVue",
   data() {
          return {
                 github: 'https://github.com/FabriGinseng',
                 mail: 'mailto:antoniofabriziofiume95@gmail.com',
                 linkedin: 'https://www.linkedin.com/in/antonio-fabrizio-fiume-13345a160',
          }
      }
};
</script>
