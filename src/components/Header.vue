<template>
  <div class="main">
    <div class="text">
      <img class="logo" src="../assets/logo.png" alt="Stake House logo">
      <h2>We run nodes.</h2>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
  props: {
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.main {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  color: black;
  align-items: stretch;
}
.text {
  color: black;
  font-size: 2em;
  text-align: center;
}

.logo {
  width: 75vw;
}
</style>
