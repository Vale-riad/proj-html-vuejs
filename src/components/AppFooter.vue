<script>
export default {
  name: "AppFooter",
  data() {
    return {
      links: [
        {
          text: "Home",
        },
        {
          text: "Meet The Band",
        },
        {
          text: "Live Dates",
        },
        {
          text: "Latest News",
        },
        {
          text: "Albums",
        },
        {
          text: "Fans",
        },
      ],
    };
  },
};
</script>

<template>
  <footer>
    <div class="footer-top">
      <div class="logo">
        <img src="../assets/avada-music-logo.png" />
      </div>
      <ul class="link">
        <li v-for="(link, index) in links">
          <a href="#">{{ link.text }}</a>
        </li>
      </ul>
    </div>
    <div class="footer-bottom">
      <div class="copyright">
        <a href="#">© Copyright 2012-2020 |</a>
        <a href="#">AVADA THEME BY THE THEMEFUSION |</a>
        <a href="#">ALLA RIGHTS RESERVED |</a>
        <a href="#">POWERED BY WORDPRESS</a>
      </div>
      <div class="icons">
        <a class="square" href="#"
          ><i class="fa-brands fa-facebook-f icon"></i
        ></a>
        <a class="square" href="#"><i class="fa-brands fa-twitter icon"></i></a>
        <a class="square" href="#"
          ><i class="fa-brands fa-instagram icon"></i
        ></a>
        <a class="square" href="#"><i class="fa-brands fa-youtube icon"></i></a>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
.footer-top {
  background-color: #323844;
  padding: 40px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  img {
    height: 60px;
  }
  ul {
    display: flex;
    list-style: none;
  }
  a {
    text-decoration: none;
    padding: 5px;
    color: #7d7b8d;
  }
  a {
    font-size: 14px;
  }
}
.footer-bottom {
  background-color: #252a33;
  padding: 40px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  a {
    color: #7d7b8d;
    padding: 5px;
    font-size: 10px;
    text-decoration: none;
  }
  .icon {
    font-size: 14px;
    color: #7d7b8d;
  }
  .square {
    height: 300px;
    width: 300px;
    background-color: #323844;
    padding: 10px 10px 10px 10px;
    margin: 5px;
  }
}
</style>
