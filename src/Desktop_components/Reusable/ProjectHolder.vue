<template>
  <slot>
    <div :class="holderClass">
      <div class="textHolderProj">
        <h3>
          Current Project:
          <a :href="link" target="_blank">
            {{ title }}
          </a>
        </h3>
        <h5>&emsp;{{ description }}</h5>
      </div>
      <img :src="img" class="ProjImg" />
    </div>
  </slot>
</template>

<script>
export default {
  name: "ProjHolder",
  setup() {},
  props: {
    leftOrientation: Boolean,
    description: String,
    title: String,
    img: String,
    link: String,
  },
  computed: {
    holderClass() {
      return this.leftOrientation ? "allHolderProj" : "allHolderProjLeft";
    },
  },
};
</script>

<style>
.allHolderProj {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  margin: 5%;
}

.allHolderProjLeft {
  display: flex;
  flex-direction: row-reverse;
  justify-content: space-between;
  margin: 5%;
}

.textHolderProj {
  display: flex;
  flex-direction: column;
  text-align: left;
  width: 60%;
}

h5 {
  margin-left: 1rem;
}

.ProjImg {
  /* aspect-ratio: "original" !important; */
  max-height: 12rem;
  width: auto;
  border-radius: 1rem;
  margin-right: 5%;
  margin-left: 5%;
}
</style>
