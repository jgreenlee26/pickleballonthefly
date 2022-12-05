<script setup lang="ts">
import { useAuthUserStore } from "./stores/AuthUserStore";

const authUserStore = useAuthUserStore();
authUserStore.initUser();
</script>

<template>
  <Navbar />
  <Drawer />
  <Alerts />
</template>
