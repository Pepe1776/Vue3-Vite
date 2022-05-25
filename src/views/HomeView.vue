<script lang="ts" setup>
import { Icon } from "@iconify/vue";

</script>

<template class="main" id="app">
  <main class="main_cont">
    <div class="title-bubble"></div>
    <img class="img-bg" src="../assets/outrun-wallpaper.jpg" />
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
      <h3 class="links-title">Current Projects in the works</h3>
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
    <div class="footer">
      <a href="https://twitter.com/JNotquery" class="">
        <Icon class="bolt linki" style="font-size: 4em" icon="logos-twitter" />
      </a>
      <a href="https://instagram.com/J_Not_query" class="">
        <Icon
          class="bolt linki"
          style="font-size: 4em"
          icon="logos-instagram"
        />
      </a>
      <a href="https://www.linkedin.com/in/justin-parker-849356178/" class="">
        <Icon class="bolt linki" style="font-size: 4em" icon="logos-linkedin" />
      </a>
    </div>
    <div class="footer2">
      <h3 class="footer2-text">Made by J Parker</h3>
    </div>
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
  margin-top: 45%;
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
  /* background-color: #81f0ff; */
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
.links-title {
  font-family: "Anton", sans-serif;
   border: #00d0ff solid 2px;
  font-size: 2.3rem;
  padding: 10px;
  color: rgba(0, 0, 0, 0.74);
  text-shadow: #81f0ff 0px 4px 12px, rgb(255, 255, 255) 0px 4px 6px;
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
  text-shadow: #81ffa5 -4px 4px 8px, rgb(255, 255, 255) -4px 4px 2px;
}
.linki:hover {
  transition: all 0.5s ease-in-out;
  box-shadow: #81ffa5 5px -5px 18px, rgb(0, 110, 255) -5px 5px 25px;
}
.footer {
  position: absolute;
  top: 85%;
  left: 0%;
  padding-left: 160px;
  width: 100vw;
  height: 10%;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  z-index: 6;
  background-color: rgba(255, 255, 255, 0.207);
}
.footer2 {
  position: absolute;
  bottom: -2%;
  left: 0%;
  width: 100%;
  height: 10%;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  z-index: 6;
}
.footer2-text {
  font-family: "Anton", sans-serif;
 
  padding: 5px;
  text-align: center;
  font-size: 1.5rem;
  color: rgba(0, 0, 0, 0.74);
  flex-shrink: calc(1 - 0.5);
  text-shadow: #81f0ff 0px 4px 12px, rgb(255, 255, 255) 0px 4px 6px;
}

@media (max-width: 900px) {
  .main_cont {
    display: flex;
    height: 100vh;
    width: 100%;
  }
  .title {
    font-size: 2rem;
    margin-top: 35%;
    margin-left: -25%;
  }
  .title2 {
    font-size: 3rem;
    position: relative;
    left: -20%;
    top: 0%;
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
  .links-title {
    font-size: 2rem;
    margin-left: -8%;
    margin-top: -15%;
  }
  .links-link {
    margin-left: -2%;
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
    margin-top: 0%;
    top: 65%;
    left: 15%;
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
    margin-top: 0%;
  }
  .footer {
    font-size: 0.5rem;
    bottom: 50%;
    left: 0;
    padding: 0%;
  }
  .footer2 {

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
  top:12%;
  left: 37%;
  font-size: 3rem;
  text-shadow: #81f0ff 10px 10px 10px;
}
.header2 {
  position: absolute;
  z-index: 2;
  top: 0%;
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
  margin-top: 0%;
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
.btn3:active,
.links-link:hover,
.links-link:active {
  transition: all 0.3s ease;
  color: #a5027c;
   box-shadow: #81ffa5 5px -5px 18px, rgb(0, 110, 255) -5px 5px 25px;
  text-shadow: #00ff95 0px 4px 2px, #81f0ff 2px 6px 4px;
}
.bubble {
  position: absolute;
  top: 45%;
  left: 25%;
  transform: translate(-50%, -50%);
  /* background-color: #0395a8; */
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
  top: 55%;
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
.footer-text {
  font-size: 2rem;
  font-family: "Water Brush", cursive;
  margin-top: 3rem;
  color: #81f0ff;
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
