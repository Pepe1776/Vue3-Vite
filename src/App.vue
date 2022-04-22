<template class="main" id="app">
  <div class="main_cont">
    <div class="mode-toggle" @click="modeToggle" :class="darkDark">
      <div class="toggle">
        <div id="dark-mode" type="checkbox"></div>
      </div>
    </div>
    <div class="title_cont">
      <div class="title_cont_title">J Parker Dev</div>
    </div>
  </div>

  <div class="morph">
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
import { Icon } from "@iconify/vue";
export default {
  components: {
    Icon,
  },
  data: function () {
    return {
      isShow: false,
      isShow2: false,
      isShow3: false,
      isShow4: false,
      isShow5: false,
      isShow6: false,
      darkMode: false,
    };
  },

  props: {
    msg: String,
  },
};
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
  background-color: #fe05d936;
  color: rgb(55, 54, 54);
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
  background: ##9605fe52;
  -webkit-box-shadow: 17px 17px 24px #9605fe52, -17px -17px 24px #c1f6ff;
  box-shadow: 17px 17px 24px #9605fe52, -17px -17px 24px #fff;
  transition: height 0.7s, opacity 0.7s;
}

.btn2 {
  display: grid;
  place-items: center;
  cursor: pointer;
  color: #9605fe52;
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
  -webkit-box-shadow: 17px 17px 24px #9605fe52, -17px -17px 24px #e5fe0552;
  box-shadow: 17px 17px 24px #e5fe0552, -17px -17px 24px #e5fe0552;
}
.btn:active,
.btn:focus {
  opacity: 0.9;
  background: #e5fe0552;
  -webkit-box-shadow: 17px 17px 24px #e5fe0552, -17px -17px 24px #e5fe0552;
  box-shadow: 17px 17px 24px #e5fe0552, -17px -17px 24px #e5fe0552;
}

.btn:hover,
.btn2:hover,
.linki:hover {
  outline: 2px solid #f5f9f9;
  box-shadow: 17px 17px 24px #fa50e096, -17px -17px 24px #f1ffc1;
  opacity: 0.7;
}
.bolt {
  font-size: inherit;
}

.dial_btn {
  cursor: pointer;
  color: #9605fe52;
  border: none;
  height: 400px;
  width: 400px;
  -webkit-border-radius: 200px;
  border-radius: 200px;
  background: #9605fe52;
  -webkit-box-shadow: 17px 17px 24px #9605fe52, -17px -17px 24px #ebffc1;
  box-shadow: 17px 17px 24px #9605fe52, -17px -17px 24px #f4ffc1;
}

.btn_row {
  display: grid;
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
  background: linear-gradient(to top right, #efefef 30%, #fe05d996 400%);
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
  text-shadow: 2px 2px 8px #2e2e2e, 2px 2px 8px #c0fe0596, 4px 4px 8px #f8fafb,
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
  background: linear-gradient(145deg, #9605fe52, #f0f0f0);
  box-shadow: 15px 15px 28px #fe05d996, -15px -15px 28px #ffffff;
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
  margin: -45px 15px 0;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #ffffff97;
  background: #fe05d91f;
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
  background: #fe05d92b;
  box-shadow: 17px 17px 24px #ff37e196, -17px 17px 24px #d4ffc1;
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
  }
  .link {
    width: 100%;
    margin: 0;
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
}
body {
  background-color: #fff;
  color: #171717;
  transition: background-color 0.2s ease, color 0.2s ease;
}

body.dark-mode {
  background-color: #242424;
}
body.dark-mode .flex h1 {
  color: #fff;
}

.mode-toggle {
  position: relative;
  padding: 0;
  width: 44px;
  height: 24px;
  min-width: 36px;
  min-height: 20px;
  background-color: #262626;
  border: 0;
  border-radius: 24px;
  outline: 0;
  overflow: hidden;
  cursor: pointer;
  z-index: 2;
  -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
  -webkit-touch-callout: none;
  appearance: none;
  transition: background-color 0.5s ease;
}
.mode-toggle .toggle {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  margin: auto;
  width: 20px;
  height: 20px;
  border-radius: 50%;
  border: 3px solid transparent;
  box-shadow: inset 0 0 0 2px #a5abba;
  overflow: hidden;
  transition: transform 0.5s ease;
}
.mode-toggle .toggle #dark-mode {
  position: relative;
  width: 100%;
  height: 100%;
  overflow: hidden;
  border-radius: 50%;
}
.mode-toggle .toggle #dark-mode:before {
  content: "";
  position: relative;
  width: 100%;
  height: 100%;
  left: 50%;
  float: left;
  background-color: #a5abba;
  transition: border-radius 0.5s ease, width 0.5s ease, height 0.5s ease,
    left 0.5s ease, transform 0.5s ease;
}

body.dark-mode .mode-toggle {
  background-color: #333333;
}
body.dark-mode .mode-toggle .toggle {
  transform: translateX(19px);
}
body.dark-mode .mode-toggle .toggle #dark-mode:before {
  border-radius: 50%;
  width: 150%;
  height: 85%;
  left: 40%;
  transform: translate(-10%, -40%), rotate(-35deg);
}

html {
  font-size: 16px;
}

html,
body,
#app {
  width: 100%;
  height: 100%;
}

body {
  margin: 0;
  font-family: "Source Sans Pro";
}

h1 {
  font-weight: 400;
  transition: color 0.5s ease;
}

.flex {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100%;
}
</style>
