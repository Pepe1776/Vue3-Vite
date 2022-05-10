<script lang="ts">
// import { Icon } from "@iconify/vue";

export default {
  components: {
    // Icon,
  },
};
</script>

<template class="main" id="app">
  <main class="main_cont">
    <transition appear name="fade2" mode="out-in">
      <div class="header">
        <h1 class="title">
          Design to <br />
          Deployment
        </h1>
      </div>
    </transition>
    <div class="nav">
      <router-link class="btn3" id="tag" to="main">Projects</router-link>
      <a href="mailto:justinp@aevio.com" id="tag" class="btn3 tag">Contact</a>
    </div>
    <transition appear name="fade" mode="out-in">
      <div class="hero">
        <img src="../assets/iphone_13.png" alt="mobile" />
      </div>
    </transition>
    <transition appear name="fade" mode="out-in">
      <div class="bubble"></div>
    </transition>
    <div class="footer"></div>
  </main>
</template>

<style scoped>
@keyframes gradient {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}
 {
}
@media (max-width: 768px) {
  .main_cont {
    display: flex;
    height: 100vh;
    width: 100%;
  }
  .title {
    font-size: 3.5rem;
    margin-top: 0%;
  }
  .btn3 {
    margin: 0;
    padding: 0;
    font-size: 1.5rem;
  }
  .nav {
    font-size: 1.5rem;
    opacity: 0.3;
    position: fixed;
    margin: 0px;
    padding: 0px;
    display: flex;
    justify-content: space-evenly;
    flex-grow: calc(1 - 0.5 * (100vh - 100%));
  }
  .hero {
    flex-grow: 1;
    width: fit-content;
    margin-top: 30%;
  }
  #tag {
    font-size: 1.5rem;

  }
}

.main {
  position: relative;
  height: 100vh;
  width: 100vw;
  background-color: #efefef;
}
.main_cont {
  position: absolute;
  width: 100vw;
  height: 100vh;
  inset: 0;
  background: linear-gradient(-45deg, #70caf0, #5f74fc, #44fcb5, #f43de1);
  background-size: 400% 400%;
  animation: gradient 15s ease infinite;
  transition: background 0.3s ease-in-out;
  overflow: hidden;
}
.header {
  position: absolute;
  z-index: 2;
  top: 30%;
  left: 10%;
  font-size: 7rem;
  text-shadow: #81f0ff 10px 10px 10px;
}
.hero {
  position: absolute;
  top: 69%;
  left: 60%;
  transform: translate(-50%, -50%);
  z-index: 2;
}
.nav {
  position: absolute;
  margin-left: 3%;
}
.btn3 {
  display: inline-block;
  font-size: 3rem;
  text-shadow: #81f0ff 0px 4px 2px;
  padding: 10px;
  margin: 30px;
  cursor: pointer;
  transition: all 0.3s ease;
}
.btn3:hover,
.btn3:active {
  color: #a5027c;
  text-shadow: #00ff95 0px 4px 2px, #81f0ff 2px 6px 4px;
}
.bubble {
  position: absolute;
  top: 45%;
  left: 25%;
  transform: translate(-50%, -50%);
  background-color: #0395a8;
  width: 1200px;
  height: 500px;
  border-radius: 50%;
  z-index: 1;
  opacity: 0.2;
  filter: blur(60px);
  box-shadow: 10px 10px 30px #f6f6f6;
}
.fade-enter-active,
.fade-leave-active {
  transition: opacity 8s ease;
}

.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}
.fade2-enter-active,
.fade2-leave-active {
  transition: opacity 4s ease;
}

.fade2-enter-from,
.fade2-leave-to {
  opacity: 0;
}
.v-enter-active,
.v-leave-active {
  transition: opacity 2.5s ease;
}

.v-enter-from,
.v-leave-to {
  opacity: 0;
}
</style>
