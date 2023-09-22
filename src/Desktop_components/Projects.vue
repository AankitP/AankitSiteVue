<template>
  <div class="Content">
    <h1 class="Title">Projects<br /></h1>
    <h1 class="PageDescriptor">
      These are some of the projects that I am currently Working on, or have
      worked on in the past
    </h1>
    <div class="Projects">
      <ProjHolder
        leftOrientation="true"
        :description="HPText.ProjectPage.ProjectA.data.Description"
        :title="HPText.ProjectPage.ProjectA.data.Title"
        :img="HPText.ProjectPage.ProjectA.data.Images"
        :link="HPText.ProjectPage.ProjectA.data.Link"
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
  computed: {
    holderClass() {
      return this.leftOrientation ? "allHolderProj" : "allHolderProjLeft";
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
