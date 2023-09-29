<template>
  <div class="Content">
    <h1 class="Title">Projects<br /></h1>
    <h1 class="PageDescriptor">
      These are some of the projects that I am currently Working on, or have
      worked on in the past
    </h1>
    <div
      class="Projects"
      v-for="(text, index) in HPText.ProjectPage"
      :key="index"
    >
      <ProjHolder
        :leftOrientation="isEvenLetter(index.slice(-1)) ? true : false"
        :description="text.data.Description"
        :title="text.data.Title"
        :img="text.data.Pic"
        :link="text.data.Link"
      />
    </div>
  </div>
</template>

<script>
import HPText from "./../assets/TextFiles/SiteText.json";
import ProjHolder from "./Reusable/ProjectHolder.vue";

export default {
  name: "ProjectsDone",
  components: {
    ProjHolder: ProjHolder,
  },
  data() {
    return {
      HPText: HPText,
    };
  },
  methods: {
    isEvenLetter(letter) {
      // Check if the letter is even based on its ASCII code
      const letterCode = letter.charCodeAt(0);
      return letterCode % 2 === 0;
    },
  },
};
</script>

<style scoped>
.PageDescriptor {
  align-content: left;
  justify-content: left;
  text-align: left;
  color: #47ff94;
  font-size: 200%;
  margin-left: 3%;
}
.Title {
  align-content: left;
  justify-content: left;
  text-align: left;
  color: #10c55c;
  font-size: 500%;
}
.Content {
  color: #ffffff;
  justify-content: center;
  text-align: center;
  margin-top: 3%;
  margin-left: 4%;
  min-width: 50vw;
  width: auto;
}
</style>
