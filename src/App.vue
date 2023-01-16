<template>
  <div class="allHolder">
    <header>
      <TopBar class="topBar"/>
    </header>
    <div class="Content">
      <AboutMe class="aboutMe"/>
    </div>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import TopBar from "./components/TopBar.vue";
import AboutMe from "./components/AboutMe.vue";

export default {
  name: "App",
  components: {
    // HelloWorld,
    TopBar,
    AboutMe,
  },
};
</script>

<style scoped>

.allHolder {
  padding: 0;
  margin: 0;
  width: 100%;
  min-height: 100vh;
  background-color: #175588;
}

content {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

</style>
