<template>
  <div id="app">
    <Header :links="links" />
    <Hero />
    <Section1 />
    <Section2 />
    <Section3 />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/macro/Header.vue";
import Hero from "./components/macro/Hero.vue";
import Footer from "./components/macro/Footer.vue";
import Section1 from "./components/Sections/Section1.vue";
import Section2 from "./components/Sections/Section2.vue";
import Section3 from "./components/Sections/Section3.vue";

export default {
  name: "App",
  components: {
    Header,
    Hero,
    Section1,
    Section2,
    Section3,
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
