<template>
  <div class="modal-backdrop">
    <div class="modal">
      <header class="modal-header">
        <slot name="header"> Web3 Defi Exchange </slot>
        <button type="button" class="btn-close" @click="close">x</button>
      </header>

      <section class="modal-body">
        <slot name="body">
          Web3 Defi Exchange app exchanging test Etherum for crypto dev tokens.
          built using React, Hardhat, Ethers and Next.js
        </slot>
      </section>

      <footer class="modal-footer">
        <slot name="footer"> visit site </slot>
        <a href="https://web3-defi.netlify.app/" class="btn">
          <Icon
            class="bolt"
            style="font-size: 5.5em"
            icon="logos-metamask-icon"
          />
        </a>
      </footer>
    </div>
  </div>
</template>

<script lang="ts">
import { Icon } from "@iconify/vue";
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "ModalComp",
  methods: {
    close() {
      this.$emit("close");
    },
  },
  components: {
    Icon,
  },
};
</script>

<style>
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
  height: 75%;
  width: 75%;
  background: #abdae357;
  box-shadow: 17px 17px 24px #abdae3, -17px 17px 24px #c1f6ff;
  display: flex;
  overflow: hidden;
  flex-direction: column;
  border: 5px solid #abdae3;
}

.modal-header,
.modal-footer {
  padding: 35px;
  display: flex;
}

.modal-header {
  text-shadow: #abdae3 5px 5px 5px;
  padding: 3rem;
  display: flex;
  font-size: 3rem;
  position: relative;
  border-bottom: 1px solid #eeeeee;
  color: #eeeeee;
  justify-content: center;
  align-items: center;
}

.modal-footer {
  color: #efefef78;
  text-shadow: #abdae3 1px 1px 1px;
  display: flex;
  border-top: 1px solid #eeeeee;
  flex-direction: column;
  justify-content: flex-end;
  align-items: center;
}

.modal-body {
  color: #efefef93;
  text-shadow: #abdae3 1px 1px 1px;
  font-size: 2rem;
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

.btn-green {
  color: white;
  background: #4aae9c00;
  border: 1px solid #4aae9b;
  border-radius: 2px;
}
</style>
