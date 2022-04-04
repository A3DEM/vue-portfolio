<template>
  <HeaderComp/>
  <IntroComp/>
  <PersoComp/>
  <AboutMe/>
  <WebProjects/>
  <DesignProjects/>
  <ContactMe/>
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

export default {
  name: 'App',
  components: {
    HeaderComp,
    IntroComp,
    PersoComp,
    AboutMe,
    WebProjects,
    DesignProjects,
    ContactMe
  }
}
</script>

<style>
body {
  margin: 0;
}
#app {
  font-family: dharma-gothic-m, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: #292728;
  text-align: center;
  color: white;
  padding: 0px 50px;
}
</style>
