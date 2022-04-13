<template>
  <div id="app-child">
    <HeaderComp/>
    <TitleComp/>
    <TitlesComp/>
    <AboutComp/>
    <WebWork/>
    <DesignWork/>
    <ContactComp/>
    <FooterComp/>
  </div>
</template>

<script>

import HeaderComp from "./components/HeaderComp.vue";
import TitleComp from "./components/TitleComp.vue";
import TitlesComp from "./components/TitlesComp.vue";
import AboutComp from "./components/AboutComp.vue";
import WebWork from "./components/WebWork.vue";
import DesignWork from "./components/DesignWork.vue";
import ContactComp from "./components/ContactComp.vue";
import FooterComp from "./components/FooterComp.vue";


export default {
  name: 'App',
  components: {
    HeaderComp,
    TitleComp,
    TitlesComp,
    AboutComp,
    WebWork,
    DesignWork,
    ContactComp,
    FooterComp
}
}
</script>

<style>

@font-face {
    font-family: 'SF Pro Display';
    src: url("@/assets/fonts/sf-pro-display-regular.OTF") format("opentype");
    font-display: swap;
    font-weight: normal;
}
@font-face {
    font-family: 'SF Pro Display';
    src: url("@/assets/fonts/sf-pro-display-bold.OTF") format("opentype");
    font-display: swap;
    font-weight: bold;
}

body {
    margin: 0;
    color: black;
}
  #app {
    font-family: "SF Pro Display";
  }

  #app-child {
    padding: 65px 50px;
  }

  h1 {
    font-size: 32px;
    line-height: 17.5px;
  }

  h1 > span {
    color: gray;
    font-weight: normal;
    font-size: 16px;
  }
</style>
