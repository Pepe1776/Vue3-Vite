<script lang="ts" setup>
// import { Icon } from "@iconify/vue";
</script>

<template class="main" id="app">
  <main class="main_cont">
    <div class="title-bubble"></div>
    <img class="img-bg" src="../assets/touch.jpg" />
    <transition appear name="fade2" mode="out-in">
      <div class="header">
        <h1 class="title">Design to Deployment</h1>
      </div>
    </transition>
    <transition appear name="fade2" mode="out-in">
      <div class="header2">
        <h2 class="title2">J Parker Development</h2>
      </div>
    </transition>
    <div class="links">
      <a class="links-link" href="http://aevio-ch5.netlify.app"
        >Creston Mobile Interface</a
      >
      <a class="links-link" href="http://ancestral.vercel.app"
        >Ancestral Restaurant</a
      >
    </div>
    <div class="nav">
      <router-link class="btn3" id="tag" to="main">Older Projects</router-link>
      <a href="mailto:justinp@aevio.com" id="tag" class="btn3 tag">Contact</a>
    </div>
    <transition appear name="fade" mode="out-in">
      <div class="hero">
        <img class="hero-img" src="../assets/9gu9.gif" alt="mobile" />
      </div>
    </transition>
    <transition appear name="fade" mode="out-in">
      <div class="bubble"></div>
    </transition>
    <transition appear name="fade3" mode="out-in">
      <div class="info_bubble">
        <div class="info">
          Custom tailored websites <br />
          for any size business
        </div>
      </div>
    </transition>
    <div class="footer"></div>
  </main>
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Water+Brush&display=swap");

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

#app {
  margin: 0;
  box-sizing: border-box;
  padding: 0;
}
.img-bg {
  width: 100%;
  height: 100%;
  object-fit: cover;
  position: absolute;
  top: 0;
  left: 0;
  z-index: 1;
  opacity: 0.5;
  background-blend-mode: overlay;
}
.title {
  font-family: "Water Brush", cursive;
  font-size: 5rem;
  flex-shrink: calc(1 - 0.5);
  text-shadow: #81f0ff 0px 4px 12px, rgb(255, 255, 255) 0px 4px 6px;
}
.title2 {
  font-family: "Anton", sans-serif;
  border: #00ff95 solid 2px;
  padding: 2%;
  font-size: 2rem;
  text-align: center;
  font-size: 7rem;
  color: rgba(0, 0, 0, 0.74);
  flex-shrink: calc(1 - 0.5);
  text-shadow: #81f0ff 0px 4px 12px, rgb(255, 255, 255) 0px 4px 6px;
}
.title-bubble {
  width: 60%;
  height: 25%;
  background-color: #81f0ff;
  border-radius: 30%;
}
.links {
  position: absolute;
  top: 40%;
  left: 42%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin: auto;
  margin-left: -34%;
  z-index: 6;
}
.links-link {
  text-align: center;
  font-family: "Anton", sans-serif;
  border: #00ff95 solid 2px;
  padding: 2%;
  font-size: 2rem;
  margin: 20px;
  color: rgb(8, 25, 68);
  flex-shrink: calc(1 - 0.5);
  text-shadow: #81f0ff -4px 4px 8px, rgb(255, 255, 255) -4px 4px 2px;
}
@media (max-width: 900px) {
  .main_cont {
    display: flex;
    height: 100vh;
    width: 100%;
  }
  .title {
    font-size: 2rem;
    margin-top: 25%;
    margin-left: -20%;
  }
  .title2 {
    font-size: 3rem;
    position: relative;
    left: -15%;
    top: 10%;
  }
  .header2 {
    display: grid;
    place-items: center;
  }
  .info {
    font-size: 2rem;
    position: absolute;
    top: 110%;
    left: -125%;
    width: 100vw;
    color: #ffffffba;
  }
  .info_bubble {
    display: flex;
    width: 100vw;
  }

  .btn3 {
    margin: 0;
    padding: 0;
    font-size: 1.5rem;
  }
  .nav {
    font-size: 1.5rem;

    opacity: 0.5;
    position: fixed;
    margin-top: 10%;
    top: 75%;
    left: -15%;
    padding: 20px;
    display: flex;
    justify-content: space-evenly;
    flex-direction: column;
    flex-grow: calc(1 - 0.5 * (100vh - 100%));
  }
  .nav > a {
    border: #00ff95 solid 2px;
  }
  .hero {
    flex-grow: 1, 0;

    margin-top: 33%;
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
  top: 15%;
  left: 37%;
  font-size: 3rem;
  text-shadow: #81f0ff 10px 10px 10px;
}
.header2 {
  position: absolute;
  z-index: 2;
  top: 1%;
  left: 30%;
  text-shadow: #81f0ff 10px 10px 10px;
}
.hero {
}

.hero-img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  background-blend-mode: overlay;
  opacity: 0.5;
  margin-left: 0%;
}
.nav {
  position: absolute;
  margin-left: 3%;
  margin-top: -10%;
  z-index: 5;
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
.info_bubble {
  position: absolute;
  top: 80%;
  left: 80%;
  transform: translate(-50%, -50%);
  width: 100vw;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  z-index: 2;
  font-size: 5rem;
  font-family: "Water Brush", cursive;
  text-shadow: #81f0ff 0px 4px 12px, rgb(255, 255, 255) 0px 4px 6px;
}
.info {
}

.fade-enter-active,
.fade-leave-active {
  transition: opacity 12s ease;
}

.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}
.fade2-enter-active,
.fade2-leave-active {
  transition: opacity 8s ease;
}

.fade2-enter-from,
.fade2-leave-to {
  opacity: 0;
}
.fade3-enter-active,
.fade3-leave-active {
  transition: opacity 16s ease;
}

.fade3-enter-from,
.fade3-leave-to {
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
