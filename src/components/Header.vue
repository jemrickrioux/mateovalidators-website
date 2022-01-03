<template>
  <div class="main">
    <div class="text">
      <h1>Mateo Validators</h1>
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
  color: white;
  align-items: stretch;
}
.text {
  color: white;
  font-size: 2em;
  text-align: center;
}
</style>
