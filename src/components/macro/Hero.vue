<template>
  <section class="hero-wrapper">
    <h2>Learn At Your Own Pace!</h2>
    <p>Get teamed up with people of the same will.</p>
    <Button :label="buttonLabel" />
    <div class="image-container">
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

    <div class="hero-wrapper-bg">
      <img class="image" src="../../assets/img/wave.svg" alt="" />
    </div>
  </section>
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
.hero-wrapper {
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
    bottom: 0;
    height: inherit;
  }
  .image {
    width: 100%;
    height: 100%;
  }
}
h2 {
  font-size: 40px;
  margin-bottom: 20px;
}
p {
  color: lightgrey;
}

.image-container {
  margin-top: 50px;
  position: relative;
  z-index: 2;
  .hero-sx {
  }
  .hero-dx {
    margin-bottom: -39px;
  }

  .hero-cx {
    border-radius: 10px;
    width: 600px;
    border: 20px solid white;
    object-fit: contain;
  }
}
</style>
