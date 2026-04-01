<template>
  <div class="footer" style="color: white">
    <button class="LinkedButton">
      <a href="https://www.instagram.com/aankit_pokhrel/" target="_blank"
        ><img src="../assets/instagram.png" class="FooterImage"
      /></a>
    </button>
    <button class="LinkedButton">
      <a href="https://www.linkedin.com/in/aankit-pokhrel/" target="_blank"
        ><img src="../assets/linkedin.png" class="FooterImage"
      /></a>
    </button>
    <button class="LinkedButton">
      <a href="https://github.com/AankitP" target="_blank"
        ><img src="../assets/github-mark-white.png" class="FooterImage"
      /></a>
    </button>
    <button class="LinkedButton">
      <a href="mailto:2001aankit@gmail.com" target="_blank"
        ><img src="../assets/gmail.png" class="FooterImage"
      /></a>
    </button>
  </div>
</template>

<script>
export default {
  name: "Footer_",
  props: {},
  components: {},
  data() {
    return {};
  },
  methods: {
    OpenLink() {
      window.open("https://github.com/AankitP", "_blank");
    },
  },
};
</script>

<style scoped>
.footer {
  position: flex;
  background-color: #08355a;
  width: 100%;
  height: 4rem;
  display: flex;
  justify-content: flex-end;
}
.LinkedButton {
  background: none;
  border: none;
  font-weight: 800;
  object-fit: contain;
  width: 8rem;
}
.FooterImage {
  max-width: 40%; /* Adjust the value as needed */
  height: auto; /* Maintain aspect ratio */
  padding: 0;
  margin: 0;
}
</style>
