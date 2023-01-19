<template>
  <div class="allHolder">
    <header>
      <TopBar class="topBar" @clicked="getPage"/>
    </header>
    <MainBox>
      <home/>
    </MainBox>
    <MainBox>
      <projectsdone/>
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
import home from "./components/Home.vue";
import projectsdone from "./components/Projects.vue";

var accessThis;

// var View = {template: '<p>banana</p>'}

export default {
  name: "App",
  components: {
    TopBar,
    MainBox,
    home,
    projectsdone,
    // VuePdfEmbed,
  },
  methods: {
    getPage(value){
      // console.log(value);
      accessThis = value;
      console.log(accessThis);
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
  min-width: 100rem;
  height: auto;
  background-color: #175588;
}

</style>
