<template>
  <div class="allHolder">
    <header>
      <TopBar class="topBar" @clicked="getPage"/>
    </header>
    <MainBox>
      <HomePage v-if="accessThis == 'Home'"/>
      <ProjectsDone v-else-if="accessThis == 'Projects'"/>
      <OofPage v-else/>
    </MainBox>
  </div>
</template>

<script>
import TopBar from "./components/TopBar.vue";
import MainBox from "./components/Reusable/MainBox.vue";
import HomePage from "./components/Home.vue";
import ProjectsDone from "./components/Projects.vue";
import OofPage from "./components/404Page.vue"


export default {
  data: function(){
    return{
      accessThis: "Home"
    }
  },
  name: "App",
  components: {
    TopBar,
    MainBox,
    HomePage,
    ProjectsDone,
    OofPage,
  },
  methods: {
    getPage(value){
      this.accessThis = value;
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
