<script>
export default {
  name: "AppMain",
};
</script>

<template>
  <main>
    <!--prima parte del main-->
    <section class="main-top">
      <div class="container text-center">
        <h2>Music Is Life</h2>
        <hr class="ms-hr" />
        <span class="paragrafo">
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Itaque
          mollitia pariatur tempore expedita doloribus suscipit nihil hic enim
          omnis consectetur iusto,<br />
          recusandae quas veniam dolores natus, vel perspiciatis ut numquam.
        </span>
      </div>
    </section>
    <!--gallery con le covers e descrizione immagini-->
    <section class="main-bottom">
      <div class="container text-center">
        <h2>Latest Band News</h2>
        <hr class="ms-hr" />
        <span class="paragrafo">
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Itaque
          mollitia pariatur tempore expedita doloribus suscipit nihil hic enim
          omnis consectetur iusto,<br />
          recusandae quas veniam dolores natus, vel perspiciatis ut numquam.
        </span>
      </div>
      <!--gallery con le covers e descrizione immagini-->
      <div class="container text-center">
        <!-- covers-->
        <section class="covers">
          <!-- parte sinistra-->
          <div class="left-cover">
            <!-- cover orizzontale -->
            <div class="box-cover horizontal">
              <img src="../assets/blog_music_techo-600x300.jpg" />

              <!-- info img -->
              <div class="bottom-cover">
                <h2>Technology and music</h2>
                <p>
                  Sed sit amet sem turpis. Curabitur cursus lacinia est at
                  interdum risus id condimentum.
                </p>
              </div>

              <!-- overlay-->
              <div class="overlay">
                <h2>Technology and music</h2>
              </div>
            </div>
            <!-- cover vericale -->
            <div class="box-cover vertical left-side">
              <img src="../assets/blog-post3-600x900.jpg" />

              <div class="bottom-cover">
                <h2>While my guitar gently sweeps</h2>
                <p>
                  Sed sit amet sem turpis. Curabitur cursus lacinia est at
                  interdum risus id condimentum.
                </p>
              </div>

              <div class="overlay">
                <h2>While my guitar gently sweeps</h2>
              </div>
            </div>
            <!-- cover vericale  -->
            <div class="box-cover vertical right">
              <img src="../assets/blog-post4.jpg" />

              <div class="bottom-cover">
                <h2>It just sounds better</h2>
                <p>
                  Sed sit amet sem turpis. Curabitur cursus lacinia est at
                  interdum risus id condimentum.
                </p>
              </div>

              <div class="overlay">
                <h2>It just sounds better</h2>
              </div>
            </div>
            <!-- cover orizzontale -->
            <div class="box-cover horizontal">
              <img src="../assets/blog_flavor_rock-1200x600.jpg" />

              <div class="bottom-cover">
                <h2>The flavor of rock</h2>
                <p>
                  Sed sit amet sem turpis. Curabitur cursus lacinia est at
                  interdum risus id condimentum.
                </p>
              </div>

              <div class="overlay">
                <h2>The flavor of rock</h2>
              </div>
            </div>
          </div>

          <!-- cover parte destra -->
          <div class="right-side">
            <div class="box-cover">
              <img src="../assets/blog-post1-600x900.jpg" />

              <div class="bottom-cover">
                <h2>Taking it back to the old school</h2>
                <p>
                  Sed sit amet sem turpis. Curabitur cursus lacinia est at
                  interdum risus id condimentum.
                </p>
              </div>

              <div class="overlay">
                <h2>Taking it back to the old school</h2>
              </div>
            </div>
            <div class="box-cover">
              <img src="../assets/blog-post2-600x900.jpg" />

              <div class="bottom-cover">
                <h2>Sharing the stage with a legend</h2>
                <p>
                  Sed sit amet sem turpis. Curabitur cursus lacinia est at
                  interdum risus id condimentum.
                </p>
              </div>

              <div class="overlay">
                <h2>Sharing the stage with a legend</h2>
              </div>
            </div>
          </div>
        </section>
      </div>
    </section>

    <!--section live dates-->
    <h2>VIEW ALL LIVE DATES</h2>
  </main>
</template>

<style lang="scss" scoped>
.main-top {
  background-color: #323844;
  padding: 50px;
  color: white;
  .ms-hr {
    width: 144px;
    color: lightgray;
    margin-left: 584px;
  }
  .paragrafo {
    color: lightgray;
  }
  .paragrafo {
    font-size: 13px;
  }
}
.main-bottom {
  background-color: #252a33;
  padding: 50px;
  color: white;
  .ms-hr {
    width: 144px;
    color: lightgray;
    margin-left: 584px;
  }
  .paragrafo {
    color: lightgray;
  }
  .paragrafo {
    font-size: 13px;
  }
  .info {
    background-color: #323844;
  }
  h6 {
    color: #ec4958;
  }
  .covers {
    height: 1380px;
    margin: 50px 0;
    display: flex;
  }
  .covers .left-cover {
    margin-left: -30px;
    display: flex;
    flex-wrap: wrap;
  }
  .covers .left-cover .box-cover.horizontal {
    margin: 0 30px;
    width: 100%;
    height: 320px;
  }
  .covers .left-cover .box-cover.horizontal img {
    width: 100%;
    min-height: 100%;
  }
  .covers .left-cover .box-cover.vertical {
    flex-basis: calc(50% - 45px);
    height: 680px;
    margin: 30px 30px;
  }
  .covers .left-cover .box-cover.vertical.left-side {
    margin-right: 15px;
  }
  .covers .left-cover .box-cover.vertical.right {
    margin-left: 15px;
  }
  .covers .left-cover .box-cover.vertical img {
    height: 100%;
  }
  .covers .right-side {
    width: 460px;
    height: 100%;
    margin-top: -30px;
  }
  .covers .right-side .box-cover {
    width: 100%;
    margin: 30px 0;
    height: calc(50% - 15px);
  }
  .covers .right-side .box-cover img {
    height: 100%;
    min-width: 100%;
  }
  .box-cover {
    position: relative;
    overflow: hidden;
  }
  .box-cover .bottom-cover {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    background-color: #323844;
    text-align: left;
    padding: 30px 25px 20px 25px;
  }
  .box-cover .bottom-cover h2 {
    color: #eb4b54;
    font-size: 20px;
  }
  .box-cover .bottom-cover p {
    color: #7d7b8d;
    line-height: 32px;
    font-size: 15px;
  }
  .box-cover .overlay {
    width: 100%;
    height: 100%;
    position: absolute;
    left: -100%;
    top: 0;
    background-color: rgba(235, 75, 84, 0.7);
    transition: left 0.5s;
    display: flex;
  }
  .box-cover .overlay h2 {
    margin: auto;
    color: white;
    font-size: 16px;
  }
  .box-cover:hover .overlay {
    left: 0;
  }
}
</style>
