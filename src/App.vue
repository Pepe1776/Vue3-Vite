<template class="app" id="app" :class="isDark ? 'dark-mode' : ''">
  <div class="main_cont" :class="isDark ? 'dark-mode' : ''">
    <!-- <button @click="isDark = !isDark" class="dark-toggle">
      <Icon
        class="dark-toggle"
        style="font-size: 4em"
        icon="emojione-v1:first-quarter-moon"
      ></Icon>
    </button> -->
    <!-- <Toggle /> -->

    <div class="title_cont">
      <div class="title_cont_title">J Parker Dev</div>
    </div>
  </div>

  <div class="morph" :class="isDark ? 'dark-mode' : ''">
    <Transition :duration="1050" name="fade" appear>
      <div class="btn_row">
        <div class="title">J Parker Dev</div>
        <h3 class="proj">Projects</h3>
        <button @click="isShow5 = !isShow5" id="vue" class="btn bb4 tooltip">
          <Icon class="bolt" style="font-size: 4em" icon="logos-vue" />
          <div class="tooltiptext">Vue 3 Portfolio</div>
        </button>

        <button @click="isShow = !isShow" id="mask" class="btn bbb tooltip">
          <Icon
            class="bolt"
            style="font-size: 4em"
            icon="logos-metamask-icon"
          />
          <div class="tooltiptext">Web3 Defi Exchange</div>
        </button>
        <button @click="isShow4 = !isShow4" id="vite" class="btn bb2 tooltip">
          <Icon class="bolt" style="font-size: 4em" icon="logos-vitejs" />
          <div class="tooltiptext">Three.js Vite Portfolio</div>
        </button>
        <button @click="isShow2 = !isShow2" id="react" class="btn bb3 tooltip">
          <Icon
            class="bolt"
            style="font-size: 4em"
            icon="logos-create-react-app"
          />
          <div class="tooltiptext">Web3 DAO React</div>
        </button>

        <button @click="isShow3 = !isShow3" id="ang" class="btn bb5 tooltip">
          <Icon class="bolt" style="font-size: 4em" icon="logos-angular-icon" />
          <div class="tooltiptext">Web3Con Nft Project</div>
        </button>
        <button @click="isShow6 = !isShow6" id="fire" class="btn bb6 tooltip">
          <Icon class="bolt" style="font-size: 4em" icon="logos-firebase" />
          <div class="tooltiptext">Full C.R.U.D. Recipes</div>
        </button>
      </div>
    </Transition>

    <!-- <div class="glass">
      <h3>Display</h3>
      <h4></h4>
    </div> -->
    <div>
      <div class="dial_row">
        <h3 class="ctc">Contact</h3>
        <a href="https://twitter.com/JNotquery" class="">
          <Icon
            class="bolt linki"
            style="font-size: 4em"
            icon="logos-twitter"
          />
        </a>
        <a href="https://instagram.com/J_Not_query" class="">
          <Icon
            class="bolt linki"
            style="font-size: 4em"
            icon="logos-instagram"
          />
        </a>
        <a href="https://www.linkedin.com/in/justin-parker-849356178/" class="">
          <Icon
            class="bolt linki"
            style="font-size: 4em"
            icon="logos-linkedin"
          />
        </a>
        <svg
          class="dark-toggle"
          width="120px"
          height="148px"
          viewBox="0 0 189 88"
          version="1.1"
          xmlns="http://www.w3.org/2000/svg"
          xmlns:xlink="http://www.w3.org/1999/xlink"
          :class="isDark ? 'dark-mode' : ''"
          @click="isDark = !isDark"
        >
          <!-- Generator: Sketch 63.1 (92452) - https://sketch.com -->
          <defs>
            <circle id="path-1" cx="25" cy="25" r="25"></circle>
          </defs>
          <g
            id="Page-1"
            stroke="none"
            stroke-width="1"
            fill="none"
            fill-rule="evenodd"
          >
            <g id="dark-mode-toggle">
              <rect
                id="bg"
                fill="#364050"
                fill-rule="nonzero"
                x="0"
                y="0"
                width="189"
                height="88"
                rx="44"
              ></rect>
              <circle
                id="main-circle"
                fill="#FFFFFF"
                fill-rule="nonzero"
                cx="46"
                cy="44"
                r="25"
              ></circle>
              <g id="moon-accents" transform="translate(21.000000, 19.000000)">
                <mask id="mask-2" fill="white">
                  <use xlink:href="#path-1"></use>
                </mask>
                <use id="Mask" fill-rule="nonzero" xlink:href="#path-1"></use>
                <circle
                  id="moon-accent-2"
                  fill="#EEEEEE"
                  fill-rule="nonzero"
                  mask="url(#mask-2)"
                  cx="44"
                  cy="23"
                  r="11"
                ></circle>
                <circle
                  id="moon-accent-1"
                  fill="#EEEEEE"
                  fill-rule="nonzero"
                  mask="url(#mask-2)"
                  cx="9"
                  cy="8"
                  r="7"
                ></circle>
                <circle
                  id="moon-accent-3"
                  fill="#EEEEEE"
                  fill-rule="nonzero"
                  mask="url(#mask-2)"
                  cx="9"
                  cy="38"
                  r="10"
                ></circle>
                <circle
                  id="moon-accent-4"
                  fill="#EEEEEE"
                  fill-rule="nonzero"
                  mask="url(#mask-2)"
                  cx="24"
                  cy="15"
                  r="6"
                ></circle>
                <circle
                  id="moon-accent-5"
                  fill="#EEEEEE"
                  fill-rule="nonzero"
                  mask="url(#mask-2)"
                  cx="31.5"
                  cy="39.5"
                  r="3.5"
                ></circle>
              </g>
              <g
                id="stars"
                transform="translate(89.000000, 18.000000)"
                fill="#FFFFFF"
              >
                <polygon
                  id="Star"
                  points="6.5 9.75 2.67939586 11.7586105 3.40906632 7.50430523 0.318132644 4.49138954 4.58969793 3.87069477 6.5 0 8.41030207 3.87069477 12.6818674 4.49138954 9.59093368 7.50430523 10.3206041 11.7586105"
                ></polygon>
                <polygon
                  id="Star-Copy"
                  points="21 43 15.1221475 46.0901699 16.2447174 39.545085 11.4894348 34.9098301 18.0610737 33.954915 21 28 23.9389263 33.954915 30.5105652 34.9098301 25.7552826 39.545085 26.8778525 46.0901699"
                ></polygon>
                <polygon
                  id="Star-Copy-2"
                  points="52 8 49.648859 9.23606798 50.097887 6.61803399 48.1957739 4.76393202 50.8244295 4.38196601 52 2 53.1755705 4.38196601 55.8042261 4.76393202 53.902113 6.61803399 54.351141 9.23606798"
                ></polygon>
                <polygon
                  id="Star-Copy-3"
                  points="60 31 56.4732885 32.854102 57.1468305 28.927051 54.2936609 26.145898 58.2366442 25.572949 60 22 61.7633558 25.572949 65.7063391 26.145898 62.8531695 28.927051 63.5267115 32.854102"
                ></polygon>
              </g>
              <g
                id="clouds"
                transform="translate(24.000000, 17.000000)"
                fill="#FFFFFF"
                fill-rule="nonzero"
              >
                <path
                  d="M22.4581401,8.64610504 C22.458794,8.60836037 22.4595787,8.57068044 22.4595787,8.53280628 C22.4595787,4.92485595 19.5054963,2 15.8614938,2 C12.7211834,2 10.0935887,4.17216375 9.42701247,7.08174056 C8.80548929,6.7372476 8.08954429,6.53997828 7.32658453,6.53997828 C4.9459644,6.53997828 3.01613657,8.45077798 3.01613657,10.8077806 C3.01613657,10.9041169 3.02051764,10.9993526 3.02686038,11.0941351 C1.2595244,11.743693 0,13.42796 0,15.4038903 C0,17.9422356 2.07832643,20 4.64203597,20 L21.1974387,20 C24.402092,20 27,17.4277945 27,14.2548467 C27,11.5105566 25.0565712,9.2160949 22.4581401,8.64610504 Z"
                  id="Path"
                ></path>
                <path
                  d="M75.4581401,38.646105 C75.458794,38.6083604 75.4595787,38.5706804 75.4595787,38.5328063 C75.4595787,34.9248559 72.5054963,32 68.8614938,32 C65.7211834,32 63.0935887,34.1721638 62.4270125,37.0817406 C61.8054893,36.7372476 61.0895443,36.5399783 60.3265845,36.5399783 C57.9459644,36.5399783 56.0161366,38.450778 56.0161366,40.8077806 C56.0161366,40.9041169 56.0205176,40.9993526 56.0268604,41.0941351 C54.2595244,41.743693 53,43.42796 53,45.4038903 C53,47.9422356 55.0783264,50 57.642036,50 L74.1974387,50 C77.402092,50 80,47.4277945 80,44.2548467 C80,41.5105566 78.0565712,39.2160949 75.4581401,38.646105 Z"
                  id="Path-Copy-2"
                ></path>
                <path
                  d="M37.4466786,38.851297 C37.1439054,38.851297 36.8417385,38.8815517 36.5450288,38.9418581 C36.3212839,37.8199968 35.5979024,36.8630135 34.5822578,36.3450283 C33.5668154,35.8270431 32.3708814,35.8053165 31.3372484,36.2859402 C30.4018448,33.6974356 27.5548062,32.3609484 24.978202,33.3006723 C22.4015977,34.2403961 21.071255,37.1007872 22.0066586,39.6890888 C19.7496033,39.7607661 17.9667177,41.6375741 18.0004714,43.905866 C18.0344273,46.1743611 19.8726934,47.9963451 22.1309613,48 L37.4466786,48 C39.9612326,48 42,45.9520193 42,43.4256485 C42,40.8992777 39.9612326,38.851297 37.4466786,38.851297 Z"
                  id="Path"
                ></path>
                <path
                  d="M56.585009,4.2909511 C56.357929,4.2909511 56.1313039,4.31313789 55.9087716,4.3573626 C55.7409629,3.5346643 55.1984268,2.83287655 54.4366934,2.45302076 C53.6751116,2.07316494 52.778161,2.05723213 52.0029363,2.4096895 C51.3013836,0.511452738 49.1661047,-0.468637832 47.2336515,0.22049299 C45.3011983,0.909623811 44.3034412,3.00724393 45.0049939,4.9053318 C43.3122025,4.95789514 41.9750383,6.33422103 42.0003536,7.99763509 C42.0258205,9.66119812 43.40452,10.9973197 45.098221,11 L56.585009,11 C58.4709244,11 60,9.4981475 60,7.64547555 C60,5.79280364 58.4709244,4.2909511 56.585009,4.2909511 Z"
                  id="Path-Copy"
                ></path>
              </g>
            </g>
          </g>
        </svg>
      </div>
      <!-- modal 1 -->
      <Transition :duration="850" name="nested">
        <div v-if="isShow" class="outer">
          <div class="modal-backdrop">
            <div class="modal inner">
              <header class="modal-header">
                <slot name="header"> Web3 Defi Exchange </slot>
                <button
                  type="button"
                  class="btn-close"
                  @click="isShow = !isShow"
                >
                  x
                </button>
              </header>

              <section class="modal-body">
                <slot name="body">
                  Web3 Defi Exchange app exchanging test Etherum for crypto dev
                  tokens. built using React, Hardhat, Ethers and Next.js
                </slot>
              </section>

              <footer class="modal-footer">
                <slot name="footer"></slot>
                <a href="https://web3-defi.netlify.app/" class="btn2 tooltip">
                  <Icon
                    class="bolt"
                    style="font-size: 5.5em"
                    icon="logos-metamask-icon"
                  />
                  <div class="tooltiptext">Visit Site</div>
                </a>
              </footer>
            </div>
          </div>
        </div>
      </Transition>

      <!-- modal 2 -->
      <Transition :duration="850" name="nested">
        <div v-if="isShow2" class="outer">
          <div class="modal-backdrop">
            <div class="modal inner">
              <header class="modal-header">
                <slot name="header"> Web3 DAO </slot>
                <button
                  type="button"
                  class="btn-close"
                  @click="isShow2 = !isShow2"
                >
                  x
                </button>
              </header>

              <section class="modal-body">
                <slot name="body">
                  Web3 DAO app to join your own DAO. Built using React, Hardhat,
                  Ethers and Next.js
                </slot>
              </section>

              <footer class="modal-footer">
                <slot name="footer"> </slot>
                <a href="https://web3-dao.netlify.app/" class="btn2 tooltip">
                  <Icon
                    class="bolt"
                    style="font-size: 5.5em"
                    icon="logos-create-react-app"
                  />
                  <div class="tooltiptext">Visit Site</div>
                </a>
              </footer>
            </div>
          </div>
        </div>
      </Transition>
      <!-- modal 3 -->
      <Transition :duration="850" name="nested">
        <div v-if="isShow3" class="outer">
          <div class="modal-backdrop">
            <div class="modal inner">
              <header class="modal-header">
                <slot name="header"> Web3Con Gratitude NFT </slot>
                <button
                  type="button"
                  class="btn-close"
                  @click="isShow3 = !isShow3"
                >
                  x
                </button>
              </header>

              <section class="modal-body">
                <slot name="body">
                  Web3Con Gratitude NFT collection app to mint and collect your
                  own NFT collection of gratitude. built using React, Hardhat,
                  Ethers and Next.js
                </slot>
              </section>

              <footer class="modal-footer">
                <slot name="footer"></slot>
                <a
                  href="https://gratitude-nft.web.app/landing"
                  class="btn2 tooltip"
                >
                  <Icon
                    class="bolt"
                    style="font-size: 5.5em"
                    icon="logos-angular-icon"
                  />
                  <div class="tooltiptext">Visit Site</div>
                </a>
              </footer>
            </div>
          </div>
        </div>
      </Transition>
      <!-- modal 4 -->
      <Transition :duration="850" name="nested">
        <div v-if="isShow4" class="outer">
          <div class="modal-backdrop">
            <div class="modal inner">
              <header class="modal-header">
                <slot name="header"> J Parker 3D Portfolio </slot>
                <button
                  type="button"
                  class="btn-close"
                  @click="isShow4 = !isShow4"
                >
                  x
                </button>
              </header>

              <section class="modal-body">
                <slot name="body">
                  Three.js built 3d interactive portfolio of J Parker. built
                  using Vite and vanilla javascript.
                </slot>
              </section>

              <footer class="modal-footer">
                <slot name="footer"></slot>
                <a href="https://jparkerdev.netlify.app/" class="btn2 tooltip">
                  <Icon
                    class="bolt"
                    style="font-size: 5.5em"
                    icon="logos-vitejs"
                  />
                  <div class="tooltiptext">Visit Site</div>
                </a>
              </footer>
            </div>
          </div>
        </div>
      </Transition>

      <!-- modal 5 -->
      <Transition :duration="850" name="nested">
        <div v-if="isShow5" class="outer">
          <div class="modal-backdrop">
            <div class="modal inner">
              <header class="modal-header">
                <slot name="header"> J Parker Dev Portfolion </slot>
                <button
                  type="button"
                  class="btn-close"
                  @click="isShow5 = !isShow5"
                >
                  x
                </button>
              </header>

              <section class="modal-body">
                <slot name="body">
                  Vue3.0 built portfolio of J Parker. built using Vue, Vite and
                  tailwind css.
                </slot>
              </section>

              <footer class="modal-footer">
                <slot name="footer"> </slot>
                <a href="https://jparker.netlify.app/" class="btn2 tooltip">
                  <Icon
                    class="bolt"
                    style="font-size: 5.5em"
                    icon="logos-vue"
                  />
                  <div class="tooltiptext">Visit Site</div>
                </a>
              </footer>
            </div>
          </div>
        </div>
      </Transition>
      <!-- modal 6 -->
      <Transition :duration="850" name="nested">
        <div v-if="isShow6" class="outer">
          <div class="modal-backdrop">
            <div class="modal inner">
              <header class="modal-header">
                <slot name="header"> Book of Recipes </slot>
                <button
                  type="button"
                  class="btn-close"
                  @click="isShow6 = !isShow6"
                >
                  x
                </button>
              </header>

              <section class="modal-body">
                <slot name="body">
                  Recipe database app made to create, read, update and delete
                  recipes tied to a user and firebase database. built using Vue,
                  Vite and tailwind css.
                </slot>
              </section>

              <footer class="modal-footer">
                <slot name="footer"></slot>
                <a
                  href="https://bookofrecipes.netlify.app/"
                  class="btn2 tooltip"
                >
                  <Icon
                    class="bolt"
                    style="font-size: 5.5em"
                    icon="logos-firebase"
                  />
                  <div class="tooltiptext">Visit Site</div>
                </a>
              </footer>
            </div>
          </div>
        </div>
      </Transition>
      <!-- end of modals -->
    </div>
  </div>
</template>

<script lang="ts">
export default {
  name: "app",
  data: function () {
    return {
      isShow: false,
      isShow2: false,
      isShow3: false,
      isShow4: false,
      isShow5: false,
      isShow6: false,
      isDark: false,
    };
  },
  methods: {
    components: {},
  },
};
</script>

<script lang="ts" setup>
import { Icon } from "@iconify/vue";

defineProps({
  msg: String,
});
</script>
<style>
@import url("https://fonts.googleapis.com/css2?family=Orbitron:wght@400;900&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Raleway:ital,wght@1,100&display=swap");

#app {
  margin: 0;
  box-sizing: border-box;
  padding: 0;
  font-family: "Orbitron", sans-serif;
}
.app {
  transition: background 0.3s ease-in-out;
}

body {
  text-align: center;
  user-select: none;
}
.notShown {
  visibility: hidden !important;
}

/* tooltip */
.tooltip {
  position: relative;
  display: inline-block;
  border-bottom: 1px dotted black;
}

.tooltip .tooltiptext {
  visibility: hidden;
  width: 100%;
  background-color: #fafe0598;
  color: rgb(0, 0, 0);
  text-align: center;
  border-radius: 16px;
  padding: 5px 0;
  font-size: 1.6rem;

  /* Position the tooltip */
  position: absolute;
  bottom: -55px;
  z-index: 1;
}

.tooltip:hover .tooltiptext {
  visibility: visible;
}

/* transitions */
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s ease;
}

.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}
.slide-fade-enter-active {
  transition: all 0.3s ease-out;
}

.slide-fade-leave-active {
  transition: all 0.8s cubic-bezier(1, 0.5, 0.8, 1);
}

.slide-fade-enter-from,
.slide-fade-leave-to {
  transform: translateX(20px);
  opacity: 0;
}
/* rules that target nested elements */
.nested-enter-active .inner,
.nested-leave-active .inner {
  transition: all 0.3s ease-in-out;
}

.nested-enter-from .inner,
.nested-leave-to .inner {
  transform: translateX(30px);
  opacity: 0;
}
/* delay enter of nested element for staggered effect */
.nested-enter-active .inner {
  transition-delay: 0.25s;
}

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

/* ADD TRANSITIONS */
#bg,
#stars,
#clouds,
#main-circle,
#moon-accents {
  transition: all 0.3s ease-out;
}
/* BACKGROUND */
svg:not(.dark-mode) #bg {
  fill: #47cfff;
}
/* SUN STYLES */
svg:not(.dark-mode) #main-circle {
  transform: translateX(100px);
  fill: #fee253;
}
/* HIDE MOON ACCENTS FOR LIGHT */
svg:not(.dark-mode) #moon-accents {
  transform: translate(121px, 19px); /* 100 + 21 */
  opacity: 0;
}
/* HIDE STARS ON LIGHT MODE */
svg:not(.dark-mode) #stars {
  opacity: 0;
  transform: translate(69px, 18px);
}
/* HIDE CLOUDS ON DARK MODE */
svg.dark-mode #clouds {
  opacity: 0;
  transform: translate(54px, 17px);
}

/* buttons */
.btn {
  display: grid;
  place-items: center;
  cursor: pointer;
  color: #abdae3;
  opacity: 0.4;
  border: none;
  margin: 25px;
  font-size: 2em;
  padding: 10px;
  width: 100%;
  height: 100%;
  -webkit-border-radius: 29px;
  border-radius: 29px;
  background: #9605fe1e;
  -webkit-box-shadow: 17px 17px 24px #ffdd00, -17px -17px 24px #e5fe05cd;
  box-shadow: 17px 17px 24px #e5fe05, -17px -17px 24px #e5fe05;
  transition: height 0.7s, opacity 0.7s;
}

.btn2 {
  display: grid;
  place-items: center;
  cursor: pointer;
  color: #ffdd00;
  opacity: 0.6;
  border: none;
  margin-top: ;
  font-size: 2em;
  padding: 5px;
  width: 40%;
  height: 80%;
  -webkit-border-radius: 29px;
  border-radius: 29px;
  background: #9605fe1e;
  -webkit-box-shadow: 17px 17px 24px #ffdd00, -17px -17px 24px #e5fe05cd;
  box-shadow: 17px 17px 24px #e5fe05, -17px -17px 24px #e5fe05;
}
.btn:active,
.btn:focus {
  opacity: 0.9;
  background: #e5fe05;
  -webkit-box-shadow: 17px 17px 24px #febc05, -17px -17px 24px #febc05;
  box-shadow: 17px 17px 24px #febc05, -17px -17px 24px #febc05;
}

.btn:hover,
.btn2:hover,
.linki:hover {
  outline: 2px solid #f9f8f5;
  box-shadow: 17px 17px 24px #febc05, -17px -17px 24px #febc05;
  opacity: 0.7;
}
.bolt {
  font-size: inherit;
}

.dial_btn {
  cursor: pointer;
  color: #ffdd00;
  border: none;
  height: 400px;
  width: 400px;
  -webkit-border-radius: 200px;
  border-radius: 200px;
  background: #ffdd00;
  -webkit-box-shadow: 17px 17px 24px #ffdd00, -17px -17px 24px #ebffc1;
  box-shadow: 17px 17px 24px #ffdd00, -17px -17px 24px #f4ffc1;
}

.btn_row {
  margin-top: 15%;
  display: grid;
  place-content: center;
  grid-template-rows: 3;
  grid-template-columns: 4;
  grid-gap: 50px;
}
.bbb {
  grid-column: 1;
  grid-row: 2;
}
.bb2 {
  grid-column: 2;
  grid-row: 2;
}
.bb3 {
  grid-column: 3;
  grid-row: 2;
}
.bb4 {
  grid-column: 1;
  grid-row: 1;
}
.bb5 {
  grid-column: 2;
  grid-row: 1;
}
.bb6 {
  grid-column: 3;
  grid-row: 1;
}

.dial_row {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  align-items: space-evenly;
  margin-left: 5%;
}

.main_cont {
  position: relative;
  width: 100vw;
  height: 100vh;
  inset: 0;
  background: linear-gradient(-45deg, #d9ff00, #ffbc04, #ff5f03, #ff0000);
  background-size: 400% 400%;
  animation: gradient 15s ease infinite;
  height: 100vh;
}
.title_cont {
  position: absolute;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 32px;
  width: 70%;
  height: 7%;
  top: 6%;
  left: 14%;
}

.title_cont_title {
  display: flex;
  margin-left: 100px;
  justify-content: center;
  align-items: center;
  font-size: 5em;
  font-weight: 900;
  color: #d7d2d2;
  text-shadow: 2px 2px 8px #ff8400, 2px 2px 8px #fafe058b, 8px 8px 18px #f8fafb,
    4px 4px 8px #2e2e2e;
}

.morph {
  position: absolute;
  display: grid;
  justify-content: center;
  align-items: center;
  width: 70%;
  height: 70%;
  top: 20%;
  left: 15%;
  border-radius: 52px;
  background: linear-gradient(145deg, #8a1414b7, #1e1d1dc0);
  box-shadow: 15px 15px 28px #ff8400, -15px -15px 28px #fafe058b;
}

.glass {
  display: flex;
  justify-content: center;
  align-items: flex-start;
  height: clamp(80%, 100%, 150%);
  width: 80%;
  color: #d7d2d2;
  background: #fe05d996;
  box-shadow: 0 8px 32px 0 rgba(8, 173, 255, 0.37);
  backdrop-filter: blur(4px);
  -webkit-backdrop-filter: blur(4px);
  border-radius: 10px;
  border: 1px solid rgba(255, 255, 255, 0.18);
}

.proj {
  position: absolute;
  width: 45%;
  margin: -95px 12px 15px 15px;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #ffffffd2;
  background: #fef60546;
  box-shadow: 0 8px 32px 0 #fff;
  backdrop-filter: blur(4px);
  -webkit-backdrop-filter: blur(4px);
  border-radius: 10px;
  border: 1px solid rgba(255, 255, 255, 0.18);
  font-size: 1.5rem;
}

/* modal */
.modal-backdrop {
  position: fixed;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  background-color: rgba(0, 0, 0, 0.5);
  display: flex;
  justify-content: center;
  align-items: center;
}

.modal {
  border-radius: 10%;
  height: 85%;
  width: 85%;
  background: #ffc40036;
  box-shadow: 17px 17px 24px #fafe058b, -17px 17px 24px #fc934c;
  display: grid;
  border: 5px solid #ffffff96;
  backdrop-filter: blur(6px);
}

.modal-header,
.modal-footer {
  padding: 35px;
  display: flex;
}

.modal-header {
  font-family: "Raleway", sans-serif;
  text-shadow: #abdae3 5px 5px 5px;
  padding: 3rem;
  display: flex;
  font-size: 5rem;
  font-weight: bold;
  position: relative;
  border-bottom: 1px solid #eeeeee;
  color: #eeeeee;
  justify-content: center;
  align-items: center;
}

.modal-footer {
  font-family: "Raleway", sans-serif;
  font-size: 1.5rem;
  color: #efefef8f;
  text-shadow: #abdae3 1px 1px 1px;
  display: flex;
  border-top: 1px solid #eeeeee;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
}

.modal-body {
  font-family: "Raleway", sans-serif;
  color: #efefef93;
  text-shadow: #abdae3 1px 1px 1px;
  font-size: 3rem;
  font-weight: bold;
  position: relative;
  padding: 40px 100px;
}

.btn-close {
  position: absolute;
  top: 20px;
  right: 35px;
  border: none;
  font-size: 3rem;
  padding: 10px;
  cursor: pointer;
  font-weight: bold;
  color: #eeeeee;
  background: transparent;
}

.modal-backdrop {
  position: fixed;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  background-color: rgba(0, 0, 0, 0.5);
  display: flex;
  justify-content: center;
  align-items: center;
}

.btn-close {
  position: absolute;
  top: 20px;
  right: 35px;
  border: none;
  font-size: 3rem;
  padding: 10px;
  cursor: pointer;
  font-weight: bold;
  color: #eeeeee;
  background: transparent;
}
.ctc {
  display: none;
}
.title {
  display: none;
}

@media (max-device-width: 1400px) {
  .btn_row {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin: 0;
    /* margin-top: 310%; */
  }
  .ctc {
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0;
    font-weight: 900;
    color: #a29e9e;
    text-shadow: 2px 2px 8px #fe05d996;
  }
  .morph {
    position: sticky;
    height: 250vh;
    width: 100vw;
    margin: 0;
    display: flex;
    flex-direction: column;
  }
  .proj {
    display: none;
    /* display: absolute;
    left: auto;
    top: auto;
    transform: translate(-80%, -40%); */
  }
  .main_cont {
    display: none;
  }
  .modal {
    width: 100vw;
    height: 100vh;
    margin-top: 0%;
    margin-left: 0%;
  }
  .modal-header {
    font-size: 2.5rem;
    padding: 2px;
  }
  .modal-body {
    margin: 0;
    font-size: 1rem;
    padding: 20px;
  }
  .modal-footer {
    margin: 0;
    font-size: 1rem;
    padding: 0;
  }
  .btn2 {
    margin: 0;
    font-size: 1rem;
    padding: 0;
  }
  .btn-close {
    font-size: 2rem;
    padding: 5px;
    margin: 0;
  }
  .dial_row {
    flex-direction: column;
  }
  .btn {
    width: 100%;
    font-size: 2rem;
  }
  .linki {
    width: 100%;
    margin-top: 10px;
    margin-bottom: 60px;
  }
  .link {
    width: 100%;
  }
  .title_cont_title {
    position: absolute;
    inset: 0;
    z-index: 4;
    font-size: 3rem;
    transform: translate(-50%, -50%);
  }
  .title {
    font-size: 1.5rem;
    display: flex;
    justify-content: center;
    align-items: center;
    font-weight: 900;
    color: #a29e9e;
    text-shadow: 2px 2px 8px #9ae0fa;
  }
  .dark-toggle {
  }
}
.dark-mode {
  background: #1a1a1a;
   background: linear-gradient(-45deg, #566502, #2a1f02, #3b1601, #000000);
  background-size: 400% 400%;
  animation: gradient 15s ease infinite;
  color: #ffffff;
  text-shadow: #abdae3 1px 1px 1px;
}
.dark-toggle {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-left: 70px;
  margin-top: -30px;
}
</style>
