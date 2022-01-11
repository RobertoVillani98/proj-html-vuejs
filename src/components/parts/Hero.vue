<template>
  <div class="hero">
    <h2>Learn At Your Own Pace!</h2>
    <p>Get teamed up with people of the same will.</p>
    <Button :label="buttonLabel" />
    <div class="container-hero">
      <img
        class="hero-sx"
        src="../../assets/img/home-6-hero-left-person-244x300.png"
        alt=""
      />
      <img
        class="hero-cx"
        src="../../assets/img/home-6-hero-poster-final.jpg"
        alt=""
      />
      <img
        class="hero-dx"
        src="../../assets/img/home-6-hero-right-person-195x300.png"
        alt=""
      />
    </div>

    <div class="hero-bg">
      <img class="image" src="../../assets/img/wave.svg" alt="" />
    </div>
  </div>
</template>

<script>
import Button from "../button/Button.vue";
export default {
  components: { Button },
  name: "Hero",
  data() {
    return {
      buttonLabel: "Get started for free",
    };
  },
};
</script>

<style lang="scss" scoped>
.hero {
  width: 100%;
  height: 500px;
  background-color: #182154;
  position: relative;
  text-align: center;
  padding-top: 60px;
  color: white;
  &-bg {
    position: absolute;
    top: 0;
    left: 0;
    height: inherit;
  }
  .image {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
}
h2 {
  font-size: 40px;
  margin-bottom: 20px;
}
p {
  color: lightgrey;
}

.container-hero {
  display: flex;
  justify-content: center;
  margin-top: 50px;

  .hero-sx,
  .hero-dx {
    z-index: 12;
  }

  .hero-cx {
    z-index: 99;
    width: 600px;
    height: 400px;
    border: 20px solid white;
    border-radius: 10px;
    object-fit: contain;
  }
}
</style>
