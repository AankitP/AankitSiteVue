<template>
  <div class="allHolder">
    <header>
      <TopBar class="topBar"/>
    </header>
    <MainBox>
      <Home/>
    </MainBox>
    <MainBox>
      <ProjectsDone/>
    </MainBox>
    <!-- this is to embed the pdf, but it didn't work, will fix in later iteration -->
    <!-- <MainBox class="PDFHolder">
      <vue-pdf-embed :source="source1" :page="1" :width="200"/>
    </MainBox> -->
  </div>
</template>

<script>
import TopBar from "./components/TopBar.vue";
import MainBox from "./components/Reusable/MainBox.vue";
import Home from "./components/Home.vue";
import ProjectsDone from "./components/Projects.vue";
// import VuePdfEmbed from 'vue-pdf-embed';

export default {
  name: "App",
  components: {
    TopBar,
    MainBox,
    Home,
    ProjectsDone,
    // VuePdfEmbed,
  },
  data(){
    return{
      compToShow: 'Home',
      // source1: "Aankit_Pokhrel_Resume.pdf"
    }
  },
};
</script>

<style>
html{
  background-color: #175588;
  width: auto;
  height: auto;
}
body{
  background-color: #175588;
}
.allHolder {
  padding: 0 !important;
  margin: 0 !important;
  min-width: 120rem;
  height: auto;
  background-color: #175588;
}

</style>
