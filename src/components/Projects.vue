<template>
    <div class="holder">
      <div class="Content">
        <h1 class="Title">
          Projects<br/>
        </h1>
        <h1 class="PageDescriptor">
          These are some of the projects that <br/>
          I have worked on throughout my time at university
        </h1>
        <div class="Projects">
          <proj-holder>
            hello
          </proj-holder>
        </div>
      </div>
    </div>
  </template>
  
  <script>
    import ProjHolder from "./Reusable/ProjectHolder.vue";
    export default {
        name: "ProjectsDone",
        components : {
            ProjHolder,
        }
    };
  </script>
  
  
  <style scoped>
  .PageDescriptor{
    align-content: left;
    justify-content: left;
    text-align: left;
    color: #47ff94;
    font-size: 200%;
    margin-left: 3%;
  }
  .Title{
    align-content: left;
    justify-content: left;
    text-align: left;
    color: #10c55c;
    font-size: 500%;
  }
  .holder{
    margin-top: 4rem;
    margin-right: 4rem;
    margin-left: 4rem;
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