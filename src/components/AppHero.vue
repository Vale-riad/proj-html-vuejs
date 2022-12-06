<script>
export default {
  name: "AppHero",
};
</script>

<template>
  <section class="hero">
    <div>
      <p class="ms-paragraph">
        <i
          >“I just listened to it and said to myself,<br />
          “Man, I really love this<br />
          album.” Still, today, it just sounds so fresh. It sounds full of
          ideas.<br />
          These guys knew what they were doing. They’re good. And they’re<br />
          inventive. I haven’t heard anything this year that’s as inventive.
          I<br />
          don’t really expect to.”</i
        >
      </p>
    </div>
    <div>
      <img class="player" src="../assets/band_interview_play_icon.png" />
    </div>
  </section>
</template>

<style lang="scss" scoped>
.hero {
  background-image: url(../assets/home-testimonial-parallax.jpg);
  height: 700px;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  .ms-paragraph {
    color: white;
  }
  .player {
    height: 60px;
  }
}
</style>
