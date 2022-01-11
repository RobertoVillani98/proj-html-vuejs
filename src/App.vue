<template>
  <div id="app">
    <Header :links="links" />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/macro/Header.vue";
import Main from "./components/macro/Main.vue";
import Footer from "./components/macro/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
  data() {
    return {
      links: [
        {
          name: "Home",
          link: "#",
        },
        {
          name: "Pages",
          link: "#",
        },
        {
          name: "Courses",
          link: "#",
        },
        {
          name: "Features",
          link: "#",
        },
        {
          name: "Blog",
          link: "#",
        },
        {
          name: "Shop",
          link: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "./assets/style/global.scss";
</style>
