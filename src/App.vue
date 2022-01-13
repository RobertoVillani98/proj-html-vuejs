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
    <Footer :links="footerNav" :contacts="contacts" />
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

      footerNav: [
        {
          title: "Explore",
          elements: [
            {
              name: "Start here",
              link: "#",
            },
            {
              name: "Blog",
              link: "#",
            },
            {
              name: "About us",
              link: "#",
            },
          ],
        },
        {
          title: "Contacts",
          elements: [
            {
              name: "Success story",
              link: "#",
            },
            {
              name: "Courses",
              link: "#",
            },
            {
              name: "Contact us",
              link: "#",
            },
          ],
        },
        {
          title: "Information",
          elements: [
            {
              name: "Membership",
              link: "#",
            },
            {
              name: "Purchase guide",
              link: "#",
            },
            {
              name: "Privacy policy",
              link: "#",
            },
            {
              name: "Term of service",
              link: "#",
            },
          ],
        },
      ],
      contacts: {
        title: "Address",
        address: "382 NE 191st St # 87392 Miami, FL 33179-3899",
        tel: "+1(305)547-9909(9am - 5pm EST, Monday - Friday)",
        mail: "support@maxcoach.com",
      },
    };
  },
};
</script>

<style lang="scss">
@import "./assets/style/global.scss";
</style>
