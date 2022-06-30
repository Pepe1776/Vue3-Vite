<template>
  <div class="main" ref="main">
    <div class="title">J Parker Dev</div>
    <div class="nav">
      <Transition appear name="fade3" mode="out-in">
        <button @click="goto('footer')" class="btn">Projects</button>
      </Transition>
      <Transition appear name="fade3" mode="out-in">
        <button class="btn">
          <a href="mailto: justinp@aevio.com"
            >Contact Me <br />
            <span class="span">(For Freelance Work)</span></a
          >
        </button>
      </Transition>
    </div>
    <Transition appear name="fade4" mode="out-in">
      <img class="img" src="../assets/JP.png" />
    </Transition>
    <div class="info">
      <img
        data-aos="fade-up"
        data-aos-offset="200"
        data-aos-delay="50"
        data-aos-duration="1000"
        data-aos-easing="ease-in-out"
        data-aos-mirror="true"
        data-aos-once="false"
        data-aos-anchor-placement="top-center"
        class="logo"
        src="../assets/jp22.png"
        alt=""
      />
    </div>
    <div class="footer-title" ref="footer">Projects</div>
    <div
      data-aos="zoom-out-down"
      data-aos-duration="1000"
      data-aos-easing="ease-in-out"
      data-aos-mirror="true"
      data-aos-once="false"
      data-aos-anchor-placement="top-center"
      class="footer"
    >
      <a href="https://web3-dao.netlify.app/">
        <Icon
          @mouseover="active = !active"
          @mouseout="active = !active"
          @touchstart="active = !active"
          @touchend="active = !active"
          class="icon defi"
          icon="cryptocurrency-d"
        />
      </a>
      <a href="https://gratitude-nft.web.app/landing">
        <Icon
          @mouseover="active2 = !active2"
          @mouseout="active2 = !active2"
          @touchstart="active2 = !active2"
          @touchend="active2 = !active2"
          class="icon nft"
          icon="logos-metamask-icon"
        />
      </a>
      <a href="https://aevio-ch5.netlify.app/">
        <Icon
          @mouseover="active3 = !active3"
          @mouseout="active3 = !active3"
          @touchstart="active3 = !active3"
          @touchend="active3 = !active3"
          class="icon cash"
          icon="emojione-mobile-phone"
        />
      </a>
      <a href="https://jparker.netlify.app/">
        <Icon
          @mouseover="active4 = !active4"
          @mouseout="active4 = !active4"
          @touchstart="active4 = !active4"
          @touchend="active4 = !active4"
          class="icon purp"
          icon="emojione-alien-monster"
        />
      </a>
      <a href="https://ancestral.vercel.app/">
        <Icon
          @mouseover="active5 = !active5"
          @mouseout="active5 = !active5"
          @touchstart="active5 = !active5"
          @touchend="active5 = !active5"
          class="icon rec"
          icon="fxemoji-potoffood"
        />
      </a>
      <a href="https://bookofrecipes.netlify.app/">
        <Icon
          @mouseover="active6 = !active6"
          @mouseout="active6 = !active6"
          @touchstart="active6 = !active6"
          @touchend="active6 = !active6"
          class="icon anc"
          icon="emojione-shallow-pan-of-food"
        />
      </a>
      <transition appear name="fade" mode="out-in">
        <img
          v-if="active"
          class="defi-img tooltiptext"
          src="../assets/dao.jpg"
          alt="defi"
        />
      </transition>
      <transition appear name="fade2" mode="out-in">
        <h3 v-if="active" class="label label1">Web3 DAO</h3>
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
        <h3 v-if="active3" class="label label3">
          Mobile Crestron <br />
          View on Mobile only
        </h3>
      </transition>
      <transition appear name="fade" mode="out-in">
        <img
          v-if="active4"
          src="../assets/jpa.jpg"
          alt="nft"
          class="defi-img jpa-img"
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
    <div class="freelance">
      <div class="freelance-dot"></div>
      <div class="freelance-dot2"></div>
      <div class="freelance-dot3"></div>
      <div class="freelance-dot4"></div>
      <div class="freelance-dot5"></div>
      <div class="freelance-dot6"></div>
      <div class="freelance-dot7"></div>
      <div class="freelance-title">Freelance</div>
      <div
        data-aos="flip-down"
        data-aos-duration="1000"
        data-aos-easing="ease-in-out"
        data-aos-mirror="true"
        data-aos-once="false"
        data-aos-anchor-placement="top-center"
        class="freelance-bubble"
      >
        <div class="freelance-body">
          <ul>
            <li>
              <Icon
                icon="logos-ant-design"
                style="font-size: 3em; margin: 10px"
              />
              Design modern yet custom websites for clients.
            </li>
            <li>
              <Icon
                icon="logos-open-graph"
                style="font-size: 3em; margin: 10px"
              />
              Make in depth reports on how to better your existing website
            </li>
            <li>
              <Icon
                icon="logos:brandfolder-icon"
                style="font-size: 3em; margin: 10px"
              />
              Help brand your small business into a modern online presence
            </li>
          </ul>
        </div>
      </div>
    </div>
    <div class="frames">
      <h4 class="frame-title">Logo Designs</h4>
      <div class="frames2">
        <img
          data-aos="fade-right"
          data-aos-duration="1000"
          data-aos-easing="ease-in-out"
          data-aos-mirror="true"
          data-aos-once="false"
          data-aos-anchor-placement="top-center"
          id="burger"
          class="frame2"
          src="../assets/star-3.png"
          alt="web1"
        />
        <img
          data-aos="fade-left"
          data-aos-duration="1000"
          data-aos-easing="ease-in-out"
          data-aos-mirror="true"
          data-aos-once="false"
          data-aos-anchor-placement="top-center"
          id="burger"
          class="frame2"
          src="../assets/star-4.png"
          alt="web1"
        />
        <img
          data-aos="fade-right"
          data-aos-duration="1000"
          data-aos-easing="ease-in-out"
          data-aos-mirror="true"
          data-aos-once="false"
          data-aos-anchor-placement="top-center"
          id="burger"
          class="frame2"
          src="../assets/star-1.png"
          alt="web1"
        />
        <img
          data-aos="fade-left"
          data-aos-duration="1000"
          data-aos-easing="ease-in-out"
          data-aos-mirror="true"
          data-aos-once="false"
          data-aos-anchor-placement="top-center"
          id="burger"
          class="frame2"
          src="../assets/star-2.png"
          alt="web1"
        />
      </div>
      <div class="frames2">
        <img
          data-aos="fade-right"
          data-aos-duration="1000"
          data-aos-easing="ease-in-out"
          data-aos-mirror="true"
          data-aos-once="false"
          data-aos-anchor-placement="top-center"
          id="burger"
          class="frame2"
          src="../assets/unnamed3.png"
          alt="web1"
        />
        <img
          data-aos="fade-left"
          data-aos-duration="1000"
          data-aos-easing="ease-in-out"
          data-aos-mirror="true"
          data-aos-once="false"
          data-aos-anchor-placement="top-center"
          id="burger"
          class="frame2"
          src="../assets/unnamed4.png"
          alt="web1"
        />
        <img
          data-aos="fade-right"
          data-aos-duration="1000"
          data-aos-easing="ease-in-out"
          data-aos-mirror="true"
          data-aos-once="false"
          data-aos-anchor-placement="top-center"
          id="burger"
          class="frame2"
          src="../assets/unnamed5.png"
          alt="web1"
        />
        <img
          data-aos="fade-left"
          data-aos-duration="1000"
          data-aos-easing="ease-in-out"
          data-aos-mirror="true"
          data-aos-once="false"
          data-aos-anchor-placement="top-center"
          id="burger"
          class="frame2"
          src="../assets/unnamed7.png"
          alt="web1"
        />
      </div>
      <h4 class="frame-title">Ui Designs</h4>
      <img
        data-aos="fade-right"
        data-aos-duration="1000"
        data-aos-easing="ease-in-out"
        data-aos-mirror="true"
        data-aos-once="false"
        data-aos-anchor-placement="top-center"
        class="frame"
        src="../assets/av1.png"
      />
      <img
        data-aos="fade-left"
        data-aos-duration="1000"
        data-aos-easing="ease-in-out"
        data-aos-mirror="true"
        data-aos-once="false"
        data-aos-anchor-placement="top-center"
        class="frame"
        src="../assets/av2.png"
      />
      <img
        data-aos="fade-right"
        data-aos-duration="1000"
        data-aos-easing="ease-in-out"
        data-aos-mirror="true"
        data-aos-once="false"
        data-aos-anchor-placement="top-center"
        class="frame"
        src="../assets/av3.png"
      />
      <div class="frames2">
        <img
          data-aos="fade-right"
          data-aos-offset="200"
          data-aos-delay="50"
          data-aos-duration="1000"
          data-aos-easing="ease-in-out"
          data-aos-mirror="true"
          data-aos-once="false"
          data-aos-anchor-placement="top-center"
          id="burger"
          class="frame2"
          src="../assets/sws@2x.png"
          alt="web1"
        />
        <img
          data-aos="fade-left"
          data-aos-offset="200"
          data-aos-delay="50"
          data-aos-duration="1000"
          data-aos-easing="ease-in-out"
          data-aos-mirror="true"
          data-aos-once="false"
          data-aos-anchor-placement="top-center"
          id="burger"
          class="frame2"
          src="../assets/sws2@2x.png"
          alt="web1"
        />
      </div>
      <div class="frames2">
        <img
          data-aos="fade-right"
          data-aos-offset="200"
          data-aos-delay="50"
          data-aos-duration="1000"
          data-aos-easing="ease-in-out"
          data-aos-mirror="true"
          data-aos-once="false"
          data-aos-anchor-placement="top-center"
          id="burger"
          class="frame2"
          src="../assets/mondo@2x.png"
          alt="web1"
        />
        <img
          data-aos="fade-left"
          data-aos-offset="200"
          data-aos-delay="50"
          data-aos-duration="1000"
          data-aos-easing="ease-in-out"
          data-aos-mirror="true"
          data-aos-once="false"
          data-aos-anchor-placement="top-center"
          id="burger"
          class="frame2"
          src="../assets/mondo-cart@2x.png"
          alt="web1"
        />
      </div>
      <img
        data-aos="fade-right"
        data-aos-duration="1000"
        data-aos-easing="ease-in-out"
        data-aos-mirror="true"
        data-aos-once="false"
        data-aos-anchor-placement="top-center"
        class="frame"
        src="../assets/Bees-Knees.png"
      />
      <img
        data-aos="fade-left"
        data-aos-offset="200"
        data-aos-delay="50"
        data-aos-duration="1000"
        data-aos-easing="ease-in-out"
        data-aos-mirror="true"
        data-aos-once="false"
        data-aos-anchor-placement="top-center"
        class="frame"
        src="../assets/WEb5.png"
      />
      <img
        data-aos="fade-right"
        data-aos-offset="200"
        data-aos-delay="50"
        data-aos-duration="1000"
        data-aos-easing="ease-in-out"
        data-aos-mirror="true"
        data-aos-once="false"
        data-aos-anchor-placement="top-center"
        class="frame"
        src="../assets/3333.png"
      />
      <img
        data-aos="fade-left"
        data-aos-offset="200"
        data-aos-delay="50"
        data-aos-duration="1000"
        data-aos-easing="ease-in-out"
        data-aos-mirror="true"
        data-aos-once="false"
        data-aos-anchor-placement="top-center"
        class="frame"
        src="../assets/bot-net@2x.png"
      />
      <img
        data-aos="fade-right"
        data-aos-offset="200"
        data-aos-delay="50"
        data-aos-duration="1000"
        data-aos-easing="ease-in-out"
        data-aos-mirror="true"
        data-aos-once="false"
        data-aos-anchor-placement="top-center"
        class="frame"
        src="../assets/saturn@2x.png"
      />

      <img
        data-aos="fade-left"
        data-aos-offset="200"
        data-aos-delay="50"
        data-aos-duration="1000"
        data-aos-easing="ease-in-out"
        data-aos-mirror="true"
        data-aos-once="false"
        data-aos-anchor-placement="top-center"
        class="frame"
        src="../assets/UI@2x.png"
        alt="web1"
      />
    </div>

    <div class="frames2"></div>

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
  </div>
</template>
<script lang="ts" setup>
import { Icon } from "@iconify/vue";
import AOS from "aos";
import "aos/dist/aos.css";
import { ref } from "vue";
const active = ref(false);
const active2 = ref(false);
const active3 = ref(false);
const active4 = ref(false);
const active5 = ref(false);
const active6 = ref(false);
AOS.init();
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
  scroll: smooth;
}
a {
  text-decoration: none;
  color: inherit;
}
.main {
  width: 100vw;
  height: auto;
  display: flex;
  flex-direction: column;
  background: linear-gradient(-45deg, #000000, #1b1b1b, #000000, #c5fe9e);
  background-size: 400% 400%;
  animation: gradient 15s ease infinite;
  transition: background 0.3s ease-in-out;
}
.img {
  width: 100%;
  height: auto;
  object-fit: cover;
  margin-top: -8%;
  top: 0%;
  left: 0%;
  z-index: 1;
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
  opacity: 0.9;
  display: none;
}
.nav {
  width: 100%;
  display: grid;
  grid-template-columns: repeat(6, 1fr);
  margin-top: 2%;
  margin-left: 60%;
  z-index: 2;
}
.btn {
  width: 100%;
  text-shadow: #5c00fc -5px 4px 12px, rgb(5, 2, 89) -10px 4px 16px;
  font-size: 3rem;
  font-family: "Anton", cursive;
  color: #fdfcfd;
  background: transparent;
  opacity: 0.7;
  transition: all 0.3s ease-in-out;
}
.span {
  opacity: 0.7;
  font-size: 2rem;
  position: absolute;
  top: 12%;
  left: 70.3%;
  transition: all 0.3s ease-in-out;
  display: none;
}
.icon {
  width: 100%;
  text-shadow: #000000 -5px 4px 12px, rgb(255, 0, 230) -10px 4px 16px;
  border: #70caf070 solid 2px;
  border-radius: 5%;
  padding: 15px;
  font-size: 10.5rem;
  font-family: "Anton", cursive;
  color: #00ffb7;
  opacity: 0.7;
  transition: all 0.3s ease-in-out;
}

.btn:active,
.home:hover,
.btn:hover {
  opacity: 1;
  text-shadow: #ff00d0 -5px 4px 12px, rgb(255, 255, 255) -10px 14px 16px;
}
.icon:hover {
  opacity: 1;
  transform: scale(1.1);
  border: #70caf0f6 solid 3px;
  box-shadow: #ff00d0 -5px 4px 12px, rgb(255, 255, 255) -10px 4px 16px;
}
.linki:hover {
  opacity: 1;
  /* box-shadow: #ff00d0 -5px 4px 12px, rgb(255, 255, 255) -10px 14px 16px; */
  border: #ff00d0 solid 1px;
  border-radius: 5%;
  padding: 10px;
}

.info {
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 15%;
  opacity: 0.7;
  z-index: 2;
}
.logo {
  width: 50%;
  height: auto;
  object-fit: cover;
  border-radius: 30%;
  margin-top: -38%;
  z-index: 1;
  box-shadow: #ffffff -15px 14px 18px, rgb(10, 4, 192) -20px 14px 18px;
  opacity: 0.5;
}
.footer {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  margin-top: 10%;
  margin-bottom: 20%;
}
.footer-title,
.freelance-title {
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
  z-index: 2;
}
.freelance {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  margin-top: 0%;
}
li {
  width: 100%;
  text-shadow: #5c00fc -5px 4px 12px, rgb(5, 2, 89) -10px 4px 16px;
  font-size: 2.5rem;
  font-family: "Anton", cursive;
  color: #fdfcfd;
  opacity: 0.7;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 5%;
}
.freelance-bubble {
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 5%;
  background: transparent;
  box-shadow: #9e5ffc -7px 14px 12px, rgb(64, 2, 89) -15px 24px 16px;
  width: 60%;
  padding: 1rem;
  backdrop-filter: blur(10px);
  border-radius: 15%;
  border: #70caf057 solid 2px;
  z-index: 2;
}
.freelance-dot {
  position: absolute;
  top: 308%;
  left: 50%;
  background: radial-gradient(circle at 30% 30%, #a600ff, #006d77);
  box-shadow: #9e5ffc -7px 14px 12px, rgb(64, 2, 89) -15px 24px 16px;
  width: 300px;
  height: 300px;
  border-radius: 50%;
  z-index: 1;
}
.freelance-dot2 {
  position: absolute;
  top: 340%;
  left: 10%;
  background: radial-gradient(circle at 30% 30%, #00bbff, #2a0077);
  box-shadow: #9e5ffc -7px 14px 12px, rgb(64, 2, 89) -15px 24px 16px;
  width: 400px;
  height: 400px;
  border-radius: 50%;
  z-index: 0;
}
.freelance-dot3 {
  position: absolute;
  top: 140%;
  left: 65%;
  background: radial-gradient(circle at 30% 30%, #e600ff, #006777);
  box-shadow: #9e5ffc -7px 14px 12px, rgb(64, 2, 89) -15px 24px 16px;
  width: 500px;
  height: 500px;
  border-radius: 50%;
  z-index: 1;
}
.freelance-dot4 {
  position: absolute;
  top: 180%;
  left: 15%;
  background: radial-gradient(circle at 30% 30%, #9f49f6, #0004d6b9);
  box-shadow: #9e5ffc -7px 14px 12px, rgb(64, 2, 89) -15px 24px 16px;
  width: 100px;
  height: 100px;
  border-radius: 50%;
  z-index: 1;
}
.freelance-dot5 {
  position: absolute;
  top: 498%;
  left: 5%;
  background: radial-gradient(circle at 30% 30%, #49c8f6, #470052b9);
  box-shadow: #9e5ffc -7px 14px 12px, rgb(64, 2, 89) -15px 24px 16px;
  width: 300px;
  height: 300px;
  border-radius: 50%;
  z-index: 1;
}
.freelance-dot6 {
  position: absolute;
  top: 678%;
  left: 75%;
  background: radial-gradient(circle at 30% 30%, #6589f6, #dc02fefd);
  box-shadow: #9e5ffc -7px 14px 12px, rgb(64, 2, 89) -15px 24px 16px;
  width: 400px;
  height: 400px;
  border-radius: 50%;
  z-index: 0;
}

.freelance-body {
  margin-bottom: 3%;
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
  z-index: 3;
  opacity: 0.8;
  transition: all 0.3s ease-in-out;
}
.nft-img {
  left: 15%;
  z-index: 5;
}
.aev-img {
  left: 40%;
  height: 100%;
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
  top: 180%;
  left: 8%;
  z-index: 1;
}
.label2 {
  position: absolute;
  top: 180%;
  left: 21.5%;
  z-index: 1;
}
.label3 {
  position: absolute;
  text-align: center;
  top: 150%;
  left: 34%;
  z-index: 1;
}
.label4 {
  position: absolute;
  top: 180%;
  left: 51%;
  z-index: 1;
}
.label5 {
  position: absolute;
  top: 180%;
  left: 64%;
  z-index: 1;
}
.label6 {
  position: absolute;
  top: 180%;
  left: 81%;
  z-index: 1;
}
.bottom {
  width: 100%;
  text-shadow: #8ffc00 -5px 4px 12px, rgb(5, 2, 89) -10px 4px 16px;

  font-size: 2rem;
  font-family: "Anton", cursive;
  color: #beb8b9;
  opacity: 0.7;
  display: flex;
  justify-content: center;
  align-items: center;
}
.home {
  display: flex;
  justify-content: center;
  align-items: center;

  margin-bottom: 10%;
  width: 100%;
  text-shadow: #54fc00 -5px 4px 12px, rgb(5, 2, 89) -10px 4px 16px;

  font-size: 0.5rem;
  font-family: "Anton", cursive;
  color: #beb8b9;
  opacity: 0.7;
  transition: all 0.3s ease-in-out;
}
.footer-last {
  display: flex;
  justify-content: center;
  align-items: center;
  background: #ececec00;
  margin-top: 10%;
  height: auto;
  width: 100%;
  gap: 10%;
  padding: 3%;
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
  z-index: 1;

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
  gap: 5%;
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
#burger {
  object-fit: scale-down;
  width: 18%;
  z-index: 1;
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
    margin-top: 8%;
    justify-content: center;
  }
  li {
    font-size: 1rem;
  }
  .logo {
    margin-top: -25%;
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
    top: 5%;
    left: 0;
    z-index: 1;
  }
  .btn {
    width: 100%;
    font-size: 2rem;
    font-family: "Anton", cursive;
    opacity: 0.7;
    transition: all 0.3s ease-in-out;
  }
  .span {
    display: none;
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
    font-size: 0.5rem;
    margin-top: 20%;
  }
  .footer {
    flex-direction: column;
    gap: 5%;
  }
  .freelance-dot3,
  .freelance-dot,
  .freelance-dot2,
  .freelance-dot6 {
    display: none;
  }
  .footer-last {
    gap: 5%;
    font-size: 0.3rem;
  }
  .frames2 {
    flex-direction: column;
  }
  .frame2 {
    object-fit: scale-down;
    width: 50%;
    margin-top: 10%;
  }
  .frame-title {
    font-size: 3rem;
  }
  #burger {
    width: 50%;
  }
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
  transition: opacity 0.4s ease-in-out;
}

.fade2-enter-from,
.fade2-leave-to {
  opacity: 0;
}
.fade3-enter-active,
.fade3-leave-active {
  transition: opacity 5s ease-in-out;
}

.fade3-enter-from,
.fade3-leave-to {
  opacity: 0;
}
.fade4-enter-active,
.fade4-leave-active {
  transition: opacity 7s ease-in-out;
}

.fade4-enter-from,
.fade4-leave-to {
  opacity: 0;
}
</style>
