<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppLineBlue from "./components/AppLineBlue.vue";

export default {
  components: { AppHeader, AppMain, AppLineBlue },
};
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppLineBlue />
</template>

<style lang="scss">
@use "./assets/styles/general.scss";
</style>
