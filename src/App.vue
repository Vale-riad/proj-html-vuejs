<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppHero from "./components/AppHero.vue";
import AppLiveDates from "./components/AppLiveDates.vue";
import AppFooter from "./components/AppFooter.vue";
export default {
  components: {
    AppHeader,
    AppMain,
    AppHero,
    AppLiveDates,
    AppFooter,
  },
};
</script>

<template>
  <div>
    <AppHeader />
    <AppMain />
    <AppHero />
    <AppLiveDates />
    <AppFooter />
  </div>
</template>

<style lang="scss">
@import "./style/global.scss";
body {
  font-family: "Lato", sans-serif;
}
</style>
