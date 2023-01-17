<template>
  <div class="holder">
    <div class="Content">
      <h1 class="Title">Projects<br /></h1>
      <h1 class="PageDescriptor">
        These are some of the projects that <br />
        I have worked on throughout my time at university
      </h1>
      <div class="Projects">
        <ProjHolder>
            <div class="allHolderProj">
                <div class="textHolderProj">
                    <h3>Current Project: Website Refactor</h3>
                    <h5>
                    &emsp;Originally this site was written in strictly HTML and CSS (to be honest it didn't look the best).
                    At the time I did not have the knowledge to know how to make it look and function better. 
                    My schedule had started to become more hectic with classes, homework, and exams, so I had to put
                    this project on the backburner until I got the time to fix it. One day I was helping my cousin with
                    a site he was working on, and was introduced to vue, so I decided that I would fix my website.
                    </h5>
                </div>
                <img src="./../assets/IMG_5899.jpg" class="ProjImg"/>
            </div>
        </ProjHolder>
        <ProjHolder>
            <div class="allHolderProj">
                <img src="./../assets/IMG_5899.jpg"  class="ProjImg"/>
                <div class="textHolderProj">
                    <h3>Current Project: Website Refactor</h3>
                    <h5>
                    I had created a website using HTML and CSS, but it looked really
                    bad<br />
                    so I decided to recreate the site using VUE
                    </h5>
                </div>
            </div>
        </ProjHolder>
        <ProjHolder>
            <div class="allHolderProj">
                <div class="textHolderProj">
                    <h3>Current Project: Website Refactor</h3>
                    <h5>
                    I had created a website using HTML and CSS, but it looked really
                    bad<br />
                    so I decided to recreate the site using VUE
                    </h5>
                </div>
                <img src="./../assets/IMG_5899.jpg"  class="ProjImg"/>
            </div>
        </ProjHolder>
      </div>
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
.holder {
  margin-top: 4rem;
  margin-right: 4rem;
  margin-left: 4rem;
  margin-bottom: 4rem;
  min-height: 80vh;
  height: auto;
  min-width: 85vw;
  width: auto;
  display: flex;
  background-color: #08355a;
  border-radius: 1rem;
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
