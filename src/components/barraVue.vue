<template>
  <b-navbar toggleable="lg" class="shadow-lg" type="dark" variant="dark">
    <b-navbar-brand>
      <b-icon icon="person-circle" variant="light"></b-icon>
      <span class="font-weight-bold mt-auto ml-2"> Antonio Fabrizio Fiume</span>
    </b-navbar-brand>
    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
    <b-collapse id="nav-collapse" is-nav>

      <b-navbar-nav>
        <b-nav-item href="#" class="mt-auto ml-auto">
          <b-badge variant="white">
            <b-icon variant="light" icon="code-slash"></b-icon>
            <span class="text-secondary">Software developer </span>
          </b-badge>
        </b-nav-item>
        <b-nav-item
            href="https://goo.gl/maps/UjyFKjD347AcvrDk6"
            class="mt-auto ml-auto">
          <b-badge variant="white">
            <b-icon
                variant="light"
                scale="0.9"
                icon="geo-alt"
            ></b-icon>
            <span class="text-secondary">Italy. Naples </span>
          </b-badge
          ></b-nav-item>
      </b-navbar-nav>

      <b-navbar-nav class="ml-auto display-inline">
        <b-nav-item :href="github"
        ><b-icon icon="github" variant="light"></b-icon
        ></b-nav-item>
        <b-nav-item :href="mail"
        ><b-icon icon="envelope-fill" variant="light"></b-icon
        ></b-nav-item>
        <b-nav-item :href="linkedin"
        ><b-icon icon="linkedin" variant="light"></b-icon
        ></b-nav-item>
        <b-nav-item-dropdown :text="$t('changeLanguage')" right>
        <b-dropdown-item v-for="option in options"
                         :key="option.value"
                         :value="option.value"
                         @click="ChangeLanguage(option.prefix)">
          {{option.description}}
        </b-dropdown-item>
        </b-nav-item-dropdown>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>

<script>
export default {
  name: "barraVue",
   data() {
          return {
            options:[
              {
                value:1, description: this.$t('languageIT'), prefix:"it"
              },
              {
                value:2, description: this.$t('languageEN'), prefix:"en"
              }
            ],
                 github: 'https://github.com/FabriGinseng',
                 mail: 'mailto:antoniofabriziofiume95@gmail.com',
                 linkedin: 'https://www.linkedin.com/in/antonio-fabrizio-fiume-13345a160',
          }
      },
  methods:{
    ChangeLanguage(locale){
      this.$i18n.locale= locale
    }
  }
};
</script>
