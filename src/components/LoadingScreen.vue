<script lang="ts">
export default {
  name: "LoadingScreen",
};
</script>

<template>
  <div id="loading">
    <img class="img" src="../assets/777.gif" alt="loading..." width="200" />
  </div>
</template>

<style>
#loading {
  position: absolute;
  z-index: 1000;
  background-color: rgb(0, 0, 0);
  height: 100vh;
  width: 100vw;
  text-align: center;
  line-height: 100vh;
}
.img {
  position: relative;
  margin: auto;
  margin-top: -10%;
  width: 80%;
}
</style>
