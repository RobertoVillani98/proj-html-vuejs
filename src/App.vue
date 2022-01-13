<template>
  <div id="app">
    <Header :links="links" />
    <Hero />
    <Info />
    <Courses />
    <About />
    <Blogs />
    <Help />
    <Certification />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/macro/Header.vue";
import Hero from "./components/macro/Hero.vue";
import Footer from "./components/macro/Footer.vue";
import Info from "./components/Sections/Info.vue";
import Courses from "./components/Sections/Courses.vue";
import About from "./components/Sections/About.vue";
import Blogs from "./components/Sections/Blogs.vue";
import Help from "./components/Sections/Help.vue";
import Certification from "./components/Sections/Certification.vue";

export default {
  name: "App",
  components: {
    Header,
    Hero,
    Info,
    Courses,
    About,
    Blogs,
    Help,
    Certification,
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
