<script>
export default {
  name: "AppHeader",
};
</script>

<template>
  <header>
    <div class="container">
      <!--logo e menù-->
      <div class="header-top">
        <img src="../assets/avada-music-logo.png" />
        <i class="fa-solid fa-bars"></i>
      </div>
      <!--titolo e bottoni-->
      <div class="header-bottom">
        <h1 class="title">Untold Stories</h1>
        <p><em>There is an untold story behind every favourite song.</em></p>
        <div class="buttons">
          <button class="btn-red">LATEST ALBUM</button>
          <button class="btn-trasparent">LIVE DATES</button>
        </div>
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
  border-bottom: 4px solid;
  border-color: #ec4958;
  border-width: 10%;
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
    padding-top: 10px;
  }
  .buttons {
    display: flex;
    padding-top: 30px;
  }
  .btn-red {
    margin-right: 10px;
    background-color: #ec4958;
    color: #ffffff;
    border: none;
    padding: 5px 25px 5px 25px;
    font-size: 14px;
  }
  .btn-trasparent {
    border-color: lightgray;
    background-color: transparent;
    color: #ffffff;
    padding: 5px 15px 5px 15px;
  }
}
</style>
