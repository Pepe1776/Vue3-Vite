<template class="main">
  <div class="main_cont">
    <div class="title_cont">
      <div class="title_cont_title">J Parker Dev</div>
    </div>
  </div>

  <div class="morph">
    <Transition :duration="1050" name="fade" appear>
      <div class="btn_row">
        <h3 class="proj">Projects</h3>
        <button @click="isShow = !isShow" id="mask" class="btn bbb">
          <Icon
            class="bolt"
            style="font-size: 4em"
            icon="logos-metamask-icon"
          />
        </button>
        <button @click="isShow4 = !isShow4" id="vite" class="btn bb2">
          <Icon class="bolt" style="font-size: 4em" icon="logos-vitejs" />
        </button>
        <button @click="isShow2 = !isShow2" id="react" class="btn bb3">
          <Icon
            class="bolt"
            style="font-size: 4em"
            icon="logos-create-react-app"
          />
        </button>
        <button @click="isShow5 = !isShow5" id="vue" class="btn bb4">
          <Icon class="bolt" style="font-size: 4em" icon="logos-vue" />
        </button>
        <button @click="isShow3 = !isShow3" id="ang" class="btn bb5">
          <Icon class="bolt" style="font-size: 4em" icon="logos-angular-icon" />
        </button>
        <button @click="isShow6 = !isShow6" id="fire" class="btn bb6">
          <Icon class="bolt" style="font-size: 4em" icon="logos-firebase" />
        </button>
      </div>
    </Transition>
    <div class="dial_row"></div>
    <!-- <div class="glass">
      <h3>Display</h3>
      <h4></h4>
    </div> -->
    <div>
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
                <slot name="footer"> visit site </slot>
                <a href="https://web3-defi.netlify.app/" class="btn2">
                  <Icon
                    class="bolt"
                    style="font-size: 5.5em"
                    icon="logos-metamask-icon"
                  />
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
                <slot name="header"> Web3 NFT Collection </slot>
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
                  Web3 NFT collection app to mint and collect your own NFT
                  collection. built using React, Hardhat, Ethers and Next.js
                </slot>
              </section>

              <footer class="modal-footer">
                <slot name="footer"> visit site </slot>
                <a href="https://web3-defi.netlify.app/" class="btn2">
                  <Icon
                    class="bolt"
                    style="font-size: 5.5em"
                    icon="logos-create-react-app"
                  />
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
                <slot name="footer"> visit site </slot>
                <a href="https://gratitude-nft.web.app/landing" class="btn2">
                  <Icon
                    class="bolt"
                    style="font-size: 5.5em"
                    icon="logos-angular-icon"
                  />
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
                <slot name="footer"> visit site </slot>
                <a href="https://jparkerdev.netlify.app/" class="btn2">
                  <Icon
                    class="bolt"
                    style="font-size: 5.5em"
                    icon="logos-vitejs"
                  />
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
                <slot name="footer"> visit site </slot>
                <a href="https://jparker.netlify.app/" class="btn2">
                  <Icon
                    class="bolt"
                    style="font-size: 5.5em"
                    icon="logos-vue"
                  />
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
                <slot name="footer"> visit site </slot>
                <a href="https://bookofrecipes.netlify.app/" class="btn2">
                  <Icon
                    class="bolt"
                    style="font-size: 5.5em"
                    icon="logos-firebase"
                  />
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
  background: #b6e8f2;
  -webkit-box-shadow: 17px 17px 24px #abdae3, -17px -17px 24px #c1f6ff;
  box-shadow: 17px 17px 24px #334346, -17px -17px 24px #c1f6ff;
  transition: height 0.7s, opacity 0.7s;
}
.btn2 {
  display: grid;
  place-items: center;
  cursor: pointer;
  color: #abdae3;
  opacity: 0.6;
  border: none;
  margin: 25px;
  font-size: 2em;
  padding: 10px;
  width: 40%;
  height: 80%;
  -webkit-border-radius: 29px;
  border-radius: 29px;
  background: #b6e8f2;
  -webkit-box-shadow: 17px 17px 24px #abdae3, -17px -17px 24px #c1f6ff;
  box-shadow: 17px 17px 24px #abdae3, -17px -17px 24px #c1f6ff;
}
.btn:active,
.btn:focus {
  opacity: 0.9;
  background: #b6e8f2;
  -webkit-box-shadow: 17px 17px 24px #c1f6ff, -17px -17px 24px #abdae3;
  box-shadow: 17px 17px 24px #e7edee, -17px -17px 24px ##abdae3;
}

.btn:hover,
.btn2:hover {
  outline: 2px solid #f5f9f9;
  box-shadow: 17px 17px 24px #c1f6ff, -17px -17px 24px #c1f6ff;
  opacity: 0.7;
}

.dial_btn {
  cursor: pointer;
  color: #abdae3;
  border: none;
  height: 400px;
  width: 400px;
  -webkit-border-radius: 200px;
  border-radius: 200px;
  background: #b6e8f2;
  -webkit-box-shadow: 17px 17px 24px #abdae3, -17px -17px 24px #c1f6ff;
  box-shadow: 17px 17px 24px #abdae3, -17px -17px 24px #c1f6ff;
}

.btn_row {
  display: grid;
  grid-template-rows: 3;
  grid-template-columns: 4;
  grid-gap: 50px;
}
.bbb {
  grid-column: 1;
  grid-row: 1;
}
.bb2 {
  grid-column: 2;
  grid-row: 1;
}
.bb3 {
  grid-column: 3;
  grid-row: 1;
}
.bb4 {
  grid-column: 1;
  grid-row: 2;
}
.bb5 {
  grid-column: 2;
  grid-row: 2;
}
.bb6 {
  grid-column: 3;
  grid-row: 2;
}

.dial_row {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  flex-wrap: wrap;
  grid-row: 1;
  grid-column: 2;
}

.main_cont {
  position: relative;
  width: 100vw;
  height: 100vh;
  inset: 0;
  background: linear-gradient(to top right, #efefef 30%, #00d2fc 400%);
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
  font-size: 5em;
  font-weight: 900;
  color: #d7d2d2;
  text-shadow: 2px 2px 8px #9ae0fa;
}

.morph {
  position: absolute;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 70%;
  height: 70%;
  top: 20%;
  left: 15%;
  border-radius: 52px;
  background: linear-gradient(145deg, #b6e8f2, #f0f0f0);
  box-shadow: 15px 15px 28px #9ae0fa, -15px -15px 28px #ffffff;
}

.glass {
  display: flex;
  justify-content: center;
  align-items: flex-start;
  height: clamp(80%, 100%, 150%);
  width: 80%;
  color: #d7d2d2;
  background: rgba(154, 224, 250, 0.3);
  box-shadow: 0 8px 32px 0 rgba(8, 173, 255, 0.37);
  backdrop-filter: blur(4px);
  -webkit-backdrop-filter: blur(4px);
  border-radius: 10px;
  border: 1px solid rgba(255, 255, 255, 0.18);
}

.proj {
  margin-left: 139%;
  display: flex;
  justify-content: center;
  align-items: center;
  height: clamp(80%, 100%, 150%);
  width: 80%;
  color: #ffffff;
  background: rgba(154, 224, 250, 0.3);
  box-shadow: 0 8px 32px 0 rgba(8, 173, 255, 0.37);
  backdrop-filter: blur(4px);
  -webkit-backdrop-filter: blur(4px);
  border-radius: 10px;
  border: 1px solid rgba(255, 255, 255, 0.18);
  text-shadow: 2px 2px 8px #000000;
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
  background: #abdae357;
  box-shadow: 17px 17px 24px #abdae3, -17px 17px 24px #c1f6ff;
  display: grid;
  border: 5px solid #abdae3;
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
  justify-content: flex-end;
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

@media (max-device-width: 1400px) {
  .title_cont_title {
    font-size: 1.5em;
    margin-right: 50%;
  }
  .btn_row {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-right: 0%;
    /* margin-top: 310%; */
  }
  .morph {
    position: sticky;
    z-index: 2;
    margin-top: 10%;
    margin-right: 20%;
  }
  .proj {
    display: none;
  }
  .main_cont {
    display: none;
  }
  .modal {
    width: 80%;
    height: 80%;
    margin-top: 0%;
    margin-left: 0%;
  }
  .modal-header {
    font-size: 2.5rem;
    padding: 2px;
  }
  .modal-body {
    margin-top: 15%;
    font-size: 1rem;
    padding: 20px;
  }
  .modal-footer {
    margin-top: 20px;
    font-size: 1rem;
    padding: 0;
  }
  .btn2 {
    margin-top: 60px;
    font-size: 1rem;
    padding: 0;
  }
  .btn-close {
    font-size: 2rem;
    padding: 5px;
    margin-right: -10%;
    margin-top: 5%;
  }
}
</style>
