<script lang="ts">
// import { Icon } from "@iconify/vue";

export default {
  components: {
    // Icon,
  },
};
</script>

<template class="main">
  <main class="main_cont">
    <!-- <Icon
      class="bolt"
      style="font-size: 65em; opacity: 0.1"
      icon="logos-vitejs"
    /> -->

    <div class="glass">
      <h2 class="glass_title">J Parker Development</h2>
    </div>
  </main>
</template>

<style scoped>
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
  background-color: #efefef;
}
</style>
