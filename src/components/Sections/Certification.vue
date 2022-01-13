<template>
  <div class="cert">
    <div class="cert-subtitle">
      Start today for getting <span>Online Certification</span>
    </div>
    <div class="cert-title">
      You can be your own guiding star with our help!
    </div>
    <Button :label="buttonLabel2" />
  </div>
</template>

<script>
import Button from "../button/Button.vue";

export default {
  components: { Button },

  name: "Certification",
  data() {
    return {
      buttonLabel2: "Get started for free",
    };
  },
};
</script>

<style lang="scss" scoped>
.cert {
  text-align: center;
  padding: 50px 0;
  &-subtitle {
    font-size: 20px;
    margin-bottom: 10px;

    span {
      color: #27ab94;
    }
  }
  &-title {
    font-size: 30px;
  }
}
</style>