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
      <div class="header-bottom">
        <h1 class="title">Untold Stories</h1>
        <p><em>There is an untold story behind every favourite song.</em></p>
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
  height: 900px;
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
  .header-bottom {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 300px;
  }
  .title {
    flex-direction: column;
    align-items: center;
  }
  .title {
    font-size: 100px;
  }
  .title {
    color: #ffffff;
    margin-right: -20px;
  }
  p {
    color: #ffffff;
  }
}
</style>
