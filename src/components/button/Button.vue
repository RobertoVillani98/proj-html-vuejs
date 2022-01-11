<template>
  <div class="button">
    <button>{{ this.label }}</button>
  </div>
</template>

<script>
export default {
  name: "Button",
  props: ["label"],
};
</script>

<style lang="scss" scoped>
button {
  padding: 15px 40px;
  background-color: #27ab94;
  border: none;
  border-radius: 3px;
  color: white;
  font-weight: bold;
  margin-top: 30px;
}
</style>