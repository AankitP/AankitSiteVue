<template>
    <div class="Content">
      <h1 class="Title">Projects<br /></h1>
      <h1 class="PageDescriptor">
        These are some of the projects that <br />
        I am currently Working on
      </h1>
      <div class="Projects">
        <ProjHolder>
            <div class="allHolderProj">
                <div class="textHolderProj">
                    <h3>Current Project: <a href="https://github.com/AankitP/AankitSiteVue" target="_blank">Website Refactor</a></h3>
                    <h5>
                    &emsp;Originally this site was written in strictly HTML and CSS (to be honest it didn't look the best).
                    At the time I did not have the knowledge to know how to make it look and function better. 
                    My schedule had started to become more hectic with classes, homework, and exams, so I had to put
                    this project on the backburner until I got the time to fix it. One day I was helping my cousin with
                    a site he was working on, and was introduced to vue, so I decided that I would fix my website.
                    </h5>
                </div>
                <img src="./../assets/VueSiteCode.png" class="ProjImg"/>
            </div>
        </ProjHolder>
        <ProjHolder>
            <div class="allHolderProj">
                <img src="./../assets/VueSiteCode.png"  class="ProjImg"/>
                <div class="textHolderProj">
                    <h3>Current Project: <a href="https://github.com/AankitP/AankitSiteVue" target="_blank">CABStone</a></h3>
                    <h5>
                    &emsp;This project is my capstone, I am working alongside a group of 4 other people to create a 
                    modular DNS application, I am working alongside one of my other groupmates to create the front end
                    portion of the project. We are using REACT with MUI to create the front end, and GO to create the 
                    backend and modules.
                    </h5>
                </div>
            </div>
        </ProjHolder>
        <ProjHolder>
            <div class="allHolderProj">
                <div class="textHolderProj">
                    <h3>Current Project: <a href="https://github.com/AankitP/AankitSiteVue" target="_blank">Website Refactor</a></h3>
                    <h5>
                    &emsp;Originally this site was written in strictly HTML and CSS (to be honest it didn't look the best).
                    At the time I did not have the knowledge to know how to make it look and function better. 
                    My schedule had started to become more hectic with classes, homework, and exams, so I had to put
                    this project on the backburner until I got the time to fix it. One day I was helping my cousin with
                    a site he was working on, and was introduced to vue, so I decided that I would fix my website.
                    </h5>
                </div>
                <img src="./../assets/VueSiteCode.png"  class="ProjImg"/>
            </div>
        </ProjHolder>
      </div>
    </div>
</template>

<script>
import ProjHolder from "./Reusable/ProjectHolder.vue";

export default {
  name: "ProjectsDone",
  components: {
    ProjHolder: ProjHolder,
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
.ProjImg{
  height: 40%;
  width: 60%;
}
</style>