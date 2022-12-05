<script>
export default {
  name: "AppHeader",
};
</script>

<template>
  <header>
    <div class="container">
      <div class="header-top">
        <img src="../assets/avada-music-logo.png" />
        <i class="fa-solid fa-bars"></i>
      </div>
    </div>
  </header>
</template>

<style lang="scss" scoped>
header {
  padding-top: 20px;
  background-image: url(../assets/home_slider.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  height: 1000px;
  img {
    height: 50px;
  }
  .header-top {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  i {
    color: #ffffff;
  }
}
</style>
