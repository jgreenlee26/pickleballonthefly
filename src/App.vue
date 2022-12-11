<script setup lang="ts">
import { useAuthUserStore } from "./stores/AuthUserStore";

const authUserStore = useAuthUserStore();
authUserStore.initUser();
</script>

<template>
  <Navbar />
  <Drawer />
  <Alerts />
  <Footer />
</template>

<style lang="scss">
html {
    height: 100%;
  }
  body {
    background-color: #2F303A;
    height: 100%;
  }
</style>