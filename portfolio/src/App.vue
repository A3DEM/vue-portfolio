<template>

  <div id="app-child">

  <HeaderComp/>
  <IntroComp/>
  <PersoComp/>
  <AboutMe/>
  <WebProjects/>
  <DesignProjects/>
  <ContactMe/>
  </div>
  <FooterComp/>
</template>

<script>

import HeaderComp from './components/HeaderComp.vue'
import IntroComp from './components/IntroComp.vue'
import PersoComp from './components/PersoComp.vue'
// import TitleComp from './components/TitleComp.vue'
import AboutMe from './components/AboutMe.vue'
import WebProjects from './components/WebProjects.vue'
import DesignProjects from './components/DesignProjects.vue'
import ContactMe from './components/ContactMe.vue'
import FooterComp from './components/FooterComp.vue'

export default {
  name: 'App',
  components: {
    HeaderComp,
    IntroComp,
    PersoComp,
    AboutMe,
    WebProjects,
    DesignProjects,
    ContactMe,
    FooterComp
  }
}
</script>

<style>
  body {
    margin: 0;
    background-color: #292728;
    color: white;
}
  #app {
    font-family: dharma-gothic-m, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
  }

  #app-child {
    padding: 0px 50px;
  }
</style>
