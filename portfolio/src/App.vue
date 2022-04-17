<template>
  <div id="app-child" :class="mode">
    <div class="introduction">
      <HeaderComp :mode="mode" @toggle="toggle"/>
      <TitleComp/>
    </div>
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
  },
  data() {
    return {
      mode: 'light'
    }
  },
  methods: {
    toggle() {
      (this.mode === 'dark') ? this.mode = 'light': this.mode = 'dark';
    }
  },
}
</script>

<style>

@font-face {
    font-family: 'SF Pro Display';
    src: url("@/assets/fonts/sf-pro-display-regular.OTF") format("opentype");
    font-display: swap;
    font-weight: 400;
}
@font-face {
    font-family: 'SF Pro Display';
    src: url("@/assets/fonts/sf-pro-display-medium.OTF") format("opentype");
    font-display: swap;
    font-weight: 500;
}
@font-face {
    font-family: 'SF Pro Display';
    src: url("@/assets/fonts/sf-pro-display-bold.OTF") format("opentype");
    font-display: swap;
    font-weight: bold;
}

* {
  transition: all 0.3s ease-in-out;
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
  #app-child > div {
    max-width: 512px;
  }
  .dark {
    background-color: black;
  }
  .dark h1, .dark h2, .dark h3, .dark footer {
    color: white;
  }
  .light {
    background-color: white;
    color: #202020;
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

  @media screen and (min-width:1024px) {
    .introduction {
      display: grid;
      grid-template-columns: 215px 1fr;
      grid-gap: 50px;
    }
    #app-child > div {
      max-width: 1024px;
    }
  }
</style>
