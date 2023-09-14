<template>
  <div class="allHolder">
    <header>
      <TopBar class="topBar" @clicked="getPage" />
    </header>
    <MainBox>
      <HomePage v-if="accessThis == 'Home'" />
      <ProjectsDone v-else-if="accessThis == 'Projects'" />
      <ContactPage v-else-if="accessThis == 'Contact'" />
      <AboutMe v-else-if="accessThis == 'AboutMe'" />
      <OofPage v-else />
    </MainBox>
  </div>
</template>
<script>
import TopBar from "./Desktop_components/TopBar.vue";
import MainBox from "./Desktop_components/Reusable/MainBox.vue";
import HomePage from "./Desktop_components/Home.vue";
import ProjectsDone from "./Desktop_components/Projects.vue";
import ContactPage from "./Desktop_components/ContactAndSocials.vue";
import OofPage from "./Desktop_components/404Page.vue";
import AboutMe from "./Desktop_components/AboutMe.vue";

const detectDeviceType = () =>
  /Android|webOS|iPhone|iPad|iPod|BlackBerry|IEMobile|Opera Mini/i.test(
    navigator.userAgent
  )
    ? "Mobile"
    : "Desktop";
console.log(detectDeviceType()); // "Mobile" or "Desktop"

export default {
  data: function () {
    return {
      accessThis: "Home",
      isMobile: false,
    };
  },
  name: "App",
  components: {
    TopBar,
    MainBox,
    HomePage,
    ProjectsDone,
    ContactPage,
    OofPage,
    AboutMe,
  },
  methods: {
    getPage(value) {
      this.accessThis = value;
    },
  },
};
</script>

<style>
html {
  background-color: #175588;
  width: auto;
  height: auto;
}
body {
  background-color: #175588;
}
.allHolder {
  padding: 0 !important;
  margin: 0 !important;
  min-width: 100rem;
  height: auto;
  background-color: #175588;
}
</style>
