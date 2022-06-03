<template>
  <div class="main" ref="main">
    <div class="title">J Parker Dev</div>
    <div class="nav">
      <button @click="goto('footer')" class="btn">Projects</button>
      <button class="btn">
        <a href="mailto: justinp@aevio.com">Contact</a>
      </button>
    </div>
    <img class="img" src="../assets/outrun-wallpaper.jpg" />
    <div class="info">
      <img class="logo" src="../assets/image0.png" alt="" />
    </div>
    <div class="footer-title" ref="footer">Projects</div>
    <div class="footer">
      <a href="https://web3-dao.netlify.app/"
        ><Icon
          @mouseover="active = !active"
          @mouseout="active = !active"
          @touchstart="active = !active"
          @touchend="active = !active"
          class="icon defi"
          icon="cryptocurrency-d"
      /></a>
      <a href="https://gratitude-nft.web.app/landing"
        ><Icon
          @mouseover="active2 = !active2"
          @mouseout="active2 = !active2"
          @touchstart="active2 = !active2"
          @touchend="active2 = !active2"
          class="icon nft"
          icon="logos-metamask-icon"
      /></a>
      <a href="https://aevio-ch5.netlify.app/"
        ><Icon
          @mouseover="active3 = !active3"
          @mouseout="active3 = !active3"
          @touchstart="active3 = !active3"
          @touchend="active3 = !active3"
          class="icon cash"
          icon="emojione-mobile-phone"
      /></a>
      <a href="https://jparker.netlify.app/"
        ><Icon
          @mouseover="active4 = !active4"
          @mouseout="active4 = !active4"
          @touchstart="active4 = !active4"
          @touchend="active4 = !active4"
          class="icon purp"
          icon="emojione-alien-monster"
      /></a>
      <a href="https://ancestral.vercel.app/"
        ><Icon
          @mouseover="active5 = !active5"
          @mouseout="active5 = !active5"
          @touchstart="active5 = !active5"
          @touchend="active5 = !active5"
          class="icon rec"
          icon="fxemoji-potoffood"
      /></a>
      <a href="https://bookofrecipes.netlify.app/"
        ><Icon
          @mouseover="active6 = !active6"
          @mouseout="active6 = !active6"
          @touchstart="active6 = !active6"
          @touchend="active6 = !active6"
          class="icon anc"
          icon="emojione-shallow-pan-of-food"
      /></a>
      <transition appear name="fade" mode="out-in">
        <img
          v-if="active"
          class="defi-img tooltiptext"
          src="../assets/defi.jpg"
          alt="defi"
        />
      </transition>
      <transition appear name="fade2" mode="out-in">
        <h3 v-if="active" class="label label1">Web3 Defi</h3>
      </transition>
      <transition appear name="fade" mode="out-in">
        <img
          v-if="active2"
          src="../assets/nft.jpg"
          alt="nft"
          class="defi-img nft-img"
        />
      </transition>
      <transition appear name="fade2" mode="out-in">
        <h3 v-if="active2" class="label label2">Gratitude NFT</h3>
      </transition>
      <transition appear name="fade" mode="out-in">
        <img
          v-if="active3"
          src="../assets/aev.jpg"
          alt="nft"
          class="defi-img aev-img"
        />
      </transition>
      <transition appear name="fade2" mode="out-in">
        <h3 v-if="active3" class="label label3">Mobile Crestron</h3>
      </transition>
      <transition appear name="fade" mode="out-in">
        <img
          v-if="active4"
          src="../assets/jpa.jpg"
          alt="nft"
          class="defi-img jpa-img"
          label="J Parker"
        />
      </transition>
      <transition appear name="fade2" mode="out-in">
        <h3 v-if="active4" class="label label4">J Parker Portfolio</h3>
      </transition>
      <transition appear name="fade" mode="out-in">
        <img
          v-if="active5"
          src="../assets/anc.jpg"
          alt="nft"
          class="defi-img anc-img"
        />
      </transition>
      <transition appear name="fade2" mode="out-in">
        <h3 v-if="active5" class="label label5">Ancestral Restaurant</h3>
      </transition>
      <transition appear name="fade" mode="out-in">
        <img
          v-if="active6"
          src="../assets/rec.jpg"
          alt="nft"
          class="defi-img rec-img"
        />
      </transition>
      <transition appear name="fade2" mode="out-in">
        <h3 v-if="active6" class="label label6">Book of Recipes</h3>
      </transition>
    </div>
    <div class="frames">
      <h4 class="frame-title">Ui Designs</h4>
      <img class="frame" src="../assets/UI@2x.png" alt="web1" />
      <img class="frame" src="../assets/wb2.png" alt="web1" />
      <img class="frame" src="../assets/wb3.png" alt="web1" />
    </div>
    <div class="frames2">
      <img class="frame2" src="../assets/mondo@2x.png" alt="web1" />
      <img class="frame2" src="../assets/mondo-cart@2x.png" alt="web1" />
    </div>
    <div class="frames2">
      <img class="frame2" src="../assets/ip2.png" alt="web1" />
      <img class="frame2" src="../assets/ip3.png" alt="web1" />
    </div>
    <div class="footer-last">
      <a href="https://instagram.com/J_Not_query" class="">
        <Icon
          class="bolt linki"
          style="font-size: 6em"
          icon="logos-instagram"
        />
      </a>
      <a href="https://twitter.com/JNotquery" class="">
        <Icon class="bolt linki" style="font-size: 6em" icon="logos-twitter" />
      </a>

      <a href="https://www.linkedin.com/in/justin-parker-849356178/" class="">
        <Icon class="bolt linki" style="font-size: 6em" icon="logos-linkedin" />
      </a>
    </div>
    <div class="bottom">Made By J Parker Dev</div>

    <router-link to="/home" class="home">Home V1</router-link>
  </div>
</template>
<script lang="ts" setup>
import { Icon } from "@iconify/vue";
import { ref } from "vue";
const active = ref(false);
const active2 = ref(false);
const active3 = ref(false);
const active4 = ref(false);
const active5 = ref(false);
const active6 = ref(false);
</script>
<script lang="ts">
export default {
  methods: {
    goto(refName: string) {
      var element: unknown = this.$refs[refName];
      var top = element.offsetTop;

      window.scrollTo(0, top);
    },
  },
};
</script>
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

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.main {
  width: 100vw;
  height: auto;
  display: flex;
  flex-direction: column;
  background: linear-gradient(-45deg, #70caf0, #5f74fc, #961dec, #146dcb);
  background-size: 400% 400%;
  animation: gradient 15s ease infinite;
  transition: background 0.3s ease-in-out;
}
.img {
  width: 100%;
  height: auto;
  object-fit: cover;
  border-radius: 10%;
  box-shadow: #ffffff -15px 14px 18px, rgb(10, 4, 192) -20px 14px 18px;

  margin-top: -20%;
  top: 0%;
  left: 0%;
  z-index: 1;
  opacity: 0.3;
}
.title {
  width: 100%;
  display: flex;
  justify-content: center;
  margin-top: 1%;
  align-items: center;
  text-shadow: #5c00fc -5px 4px 12px, rgb(5, 2, 89) -10px 4px 16px;
  font-size: 10rem;
  font-family: "anton", cursive;
  color: #fdfcfd;
  opacity: 0.7;
}
.nav {
  width: 100%;
  display: flex;
  justify-content: space-around;
  align-items: center;
  margin-top: 1%;
  top: 15%;
  left: 0;
  z-index: 2;
}
.btn {
  width: 100%;
  text-shadow: #5c00fc -5px 4px 12px, rgb(5, 2, 89) -10px 4px 16px;
  font-size: 3rem;
  font-family: "Anton", cursive;
  color: #fdfcfd;
  opacity: 0.7;
  transition: all 0.3s ease-in-out;
}
.icon {
  width: 100%;
  text-shadow: #000000 -5px 4px 12px, rgb(255, 0, 230) -10px 4px 16px;
  border: #70caf070 solid 2px;
  padding: 15px;
  font-size: 10.5rem;
  font-family: "Anton", cursive;
  color: #00ffb7;
  opacity: 0.7;
  transition: all 0.3s ease-in-out;
}
.btn:hover,
.btn:active,
.icon:hover {
  opacity: 1;
  transform: scale(1.1);
  border: #70caf0f6 solid 3px;
}
.home:hover {
  opacity: 1;
}
.info {
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 20%;

  z-index: 1;
}
.logo {
  width: 50%;
  height: auto;
  object-fit: cover;
  border-radius: 30%;
  margin-top: -38%;
  z-index: 1;
  box-shadow: #ffffff -15px 14px 18px, rgb(10, 4, 192) -20px 14px 18px;
  opacity: 0.9;
}
.footer {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  margin-top: 5%;
  margin-bottom: 20%;
}
.footer-title {
  width: 100%;
  text-shadow: #5c00fc -5px 4px 12px, rgb(5, 2, 89) -10px 4px 16px;
  font-size: 5rem;
  font-family: "Anton", cursive;
  color: #fdfcfd;
  opacity: 0.7;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 10%;
}
.defi-img {
  width: 30%;
  height: auto;
  object-fit: cover;
  border-radius: 10%;
  margin-top: 2%;
  position: absolute;
  top: 222%;
  left: 3%;
  z-index: 1;
  opacity: 0.8;
  transition: all 0.3s ease-in-out;
}
.nft-img {
  left: 15%;
}
.aev-img {
  left: 40%;
  height: 30%;
  width: auto;
}
.jpa-img {
  left: 47%;
}
.anc-img {
  left: 63%;
}
.rec-img {
  left: 68%;
}
.label {
  font-size: 3rem;
  color: #e6e3e3;
  opacity: 0.7;
  text-shadow: #5c00fc -5px 4px 12px, rgb(5, 2, 89) -10px 4px 16px;
}
.label1 {
  position: absolute;
  top: 219%;
  left: 8%;
  z-index: 1;
}
.label2 {
  position: absolute;
  top: 219%;
  left: 21.5%;
  z-index: 1;
}
.label3 {
  position: absolute;
  top: 219%;
  left: 35.3%;
  z-index: 1;
}
.label4 {
  position: absolute;
  top: 219%;
  left: 51%;
  z-index: 1;
}
.label5 {
  position: absolute;
  top: 219%;
  left: 64%;
  z-index: 1;
}
.label6 {
  position: absolute;
  top: 219%;
  left: 81%;
  z-index: 1;
}
.bottom {
  width: 100%;
  text-shadow: #5c00fc -5px 4px 12px, rgb(5, 2, 89) -10px 4px 16px;

  font-size: 4rem;
  font-family: "Anton", cursive;
  color: #beb8b9;
  opacity: 0.7;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 10%;
}
.home {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 10%;
  margin-bottom: 10%;
  width: 100%;
  text-shadow: #5c00fc -5px 4px 12px, rgb(5, 2, 89) -10px 4px 16px;

  font-size: 3rem;
  font-family: "Anton", cursive;
  color: #beb8b9;
  opacity: 0.7;
  transition: all 0.3s ease-in-out;
}
.footer-last {
  display: flex;
  justify-content: center;
  align-items: center;
  background: linear-gradient(-45deg, #70caf0, #5f74fc, #961dec, #146dcb);
  margin-top: 10%;
  height: auto;
  width: 100%;
  gap: 10%;
  padding: 3%;
  border-radius: 50%;
}
.linki {
  width: 100%;
  padding: 1%;
  font-size: 4rem;
  opacity: 0.7;
  transition: all 0.3s ease-in-out;
}
.frames {
  width: 100%;
  height: auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 10px;
}
.frame {
  width: 60%;
  height: auto;
  object-fit: cover;
  border-radius: 5%;
  box-shadow: #843efd -5px 4px 12px, rgb(0, 162, 255) -10px 4px 16px;

  margin-top: 10%;
  opacity: 0.8;
  transition: all 0.3s ease-in-out;
}
.frame2 {
  width: auto;
  height: 100%;
  border-radius: 5%;
  box-shadow: #843efd -5px 4px 12px, rgb(0, 162, 255) -10px 4px 16px;
  object-fit: contain;
}
.frames2 {
  width: auto;
  height: 100%;
  display: flex;
  margin-top: 10%;
  object-fit: cover;
  justify-content: center;
  align-items: center;
  gap: 10%;
}
.frame-title {
  width: 100%;
  text-shadow: #5c00fc -5px 4px 12px, rgb(5, 2, 89) -10px 4px 16px;
  font-size: 5rem;
  font-family: "Anton", cursive;
  color: #fdfcfd;
  opacity: 0.7;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 10%;
}
@media (max-width: 768px) {
  .img {
    width: 80%;
    height: auto;
    object-fit: cover;
    border-radius: 10%;
    margin: auto;
    z-index: 1;
    opacity: 0.7;
    margin-right: 10%;
    margin-top: 15%;
    justify-content: center;
  }
  .logo {
    margin-top: 0%;
  }
  .title {
    width: 100%;
    display: flex;
    justify-content: center;
    margin-top: 1%;
    align-items: center;
    font-size: 4rem;
    font-family: "Anton", cursive;

    opacity: 0.7;
  }
  .nav {
    width: 100%;
    display: flex;
    justify-content: space-around;
    align-items: center;
    margin-top: 10%;
    top: 15%;
    left: 0;
    z-index: 1;
  }
  .btn {
    width: 100%;
    font-size: 3rem;
    font-family: "Anton", cursive;
    opacity: 0.7;
    transition: all 0.3s ease-in-out;
  }
  .icon {
    width: 100%;
    text-shadow: #000000 -5px 4px 12px, rgb(255, 0, 230) -10px 4px 16px;
    font-size: 7.5rem;
    font-family: "Anton", cursive;
    color: #00ffb7;
    opacity: 0.7;
    margin-top: 5%;
    transition: all 0.3s ease-in-out;
  }
  .bottom,
  .home {
    font-size: 2rem;
  }
  .footer {
    flex-direction: column;
    gap: 5%;
  }
  .footer-last {
    gap: 5%;
    font-size: 0.5rem;
  }
  .frames2 {
    flex-direction: column;
  }
  .frame2 {
    object-fit: scale-down;
    width: 50%;
    margin-top: 10%;
  }
}
.btn:hover,
.btn:active,
.icon:hover {
  opacity: 1;
  transform: scale(1.1);
}
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.3s ease-in-out;
}

.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}
.fade2-enter-active,
.fade2-leave-active {
  transition: opacity 1s ease-in-out;
}

.fade2-enter-from,
.fade2-leave-to {
  opacity: 0;
}
</style>
