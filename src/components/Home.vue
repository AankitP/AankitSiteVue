<template>
  <div class="aboutMe">
    <p class="helloWorld">Hello World, My Name is</p>
    <h1 class="myName">Aankit Pokhrel.<br /></h1>
    <h1 class="hook">And I Build Things for Fun.</h1>
    <div class="shortDescription">
      <p>
        I am A senior Cyber Engineering Major at Louisiana Tech university<br />
        currently a working on my capstone<br />
        and am Projected to graduate in May 2023
      </p>
    </div>
  </div>
  <div class="picOfMe">
    <img src="./../assets/IMG_5899.jpg" />
  </div>
</template>

<script>
export default {
  name: "AboutMe",
};
</script>

<style scoped>
.helloWorld {
  align-content: left;
  justify-content: left;
  text-align: left;
  color: aquamarine;
  font-size: 200%;
}
.hook {
  align-content: left;
  justify-content: left;
  text-align: left;
  color: #47ff94;
  font-size: 400%;
}
.myName {
  align-content: left;
  justify-content: left;
  text-align: left;
  color: #10c55c;
  font-size: 500%;
}

.aboutMe {
  color: #ffffff;
  justify-content: center;
  text-align: center;
  margin: 3rem;
  min-width: 50vw;
  width: auto;
}
.shortDescription {
  margin: 4.5rem;
  margin-top: 0rem;
  width: 65vw;
  height: 20rem;
  text-align: left;
}

.picOfMe {
  max-height: 40rem;
  max-width: 25rem;
  margin-right: 10vw;
}

img {
  max-height: 100%;
  max-width: 100%;
  border-radius: 10%;
  display: block;
  aspect-ratio: "1.33" !important;
}
</style>
