<template>
  <div id="blog">
    <NavBar></NavBar>
    <Main></Main>
    <Project></Project>
    <Blog></Blog>
    <About></About>
    <Contact></Contact>
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
import NavBar from "./components/Navbar";
import Main from "./components/Main";
import Project from "./components/Project";
import Blog from "./components/Blog";
import About from "./components/About";
import Contact from "./components/Contact";
import { onMounted, onUnmounted } from "vue";
import { gsap } from "gsap";
export default {
  name: "App",
  components: {
    Main,
    NavBar,
    Project,
    Blog,
    About,
    Contact,
  },
  // setup() {
  //   onMounted((el, binding) => {
  //     let f = function (evt) {
  //       if (binding.value(evt, el)) {
  //         window.removeEventListener("scroll", f);
  //       }
  //     };
  //     window.addEventListener("scroll", f);
  //     // window.addEventListener("scroll", handleScroll)
  //   }),
  //     onUnmounted(() => {
  //       window.removeEventListener("scroll", handleScroll);
  //     });
  // },
  // methods: {
  //   handleScroll(evt, el) {
  //     if (window.scrollY > 50) {
  //       gsap.to(el, {
  //         duration: 1.5,
  //         y: -10,
  //         opacity: 1,
  //         ease: "sine",
  //       });
  //     }
  //     return window.scrollY > 100;
  //   },
  // },
  setup() {
    // ...

    onMounted(() => {
      window.addEventListener("scroll", handleScroll);
    });

    onUnmounted(() => {
      window.removeEventListener("scroll", handleScroll);
    });
    const handleScroll = (el) => {
      if (window.scrollY > 50) {
        gsap.to(el, {
          duration: 1.5,
          y: -10,
          opacity: 1,
          ease: "sine",
        });
      }
      return window.scrollY > 100;
    };
    // ...
  },
};
</script>

<style lang="scss">
body {
  margin: 0;
  // height: 100%;
  // width: 100%;
  overflow-x: hidden;
}
#app {
  @import "./scss/_base.scss";
  // @import "./scss/_mixins.scss";
  font-family: "Poppins", Avenir, Helvetica, Arial, sans-serif;
  // -webkit-font-smoothing: antialiased;
  // -moz-osx-font-smoothing: grayscale;
  ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
  }
  a {
    text-decoration: none;
  }
}
</style>
