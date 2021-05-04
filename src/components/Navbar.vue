<template>
  <div class="nav-container">
    <header>
      <a href="#" class="nav-container--logo">Utshav Pandey</a>
      <nav>
        <ul>
          <li><a href="#" class="nav-container--item">My Projects</a></li>
          <li><a href="#" class="nav-container--item">My Blogs</a></li>
          <li><a href="#" class="nav-container--item">About Me</a></li>
          <!-- <li><a href="#" class="nav-container--item">Hire Me</a></li> -->
        </ul>
      </nav>
    </header>
    <div class="social-header">
      <ul>
        <li>
          <a href="#" @click="openProfile(1)">
            <img
              src="../assets/icons/github.svg"
              alt="Github"
              class="logo--navIcon"
            />
          </a>
        </li>
        <li>
          <a href="#" @click="openProfile(2)">
            <img
              src="../assets/icons/linkedin.svg"
              alt="Linkedin"
              class="logo--navIcon"
          /></a>
        </li>
        <li>
          <a href="#" @click="openProfile(3)"
            ><img
              src="../assets/icons/twitter.svg"
              alt="Twitter"
              class="logo--navIcon Twitter"
          /></a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "NavBar",
  methods: {
    openProfile: function (val) {
      if (val === 1) {
        window.open("https://github.com/utpandey", "_blank");
      } else if (val === 2) {
        window.open(
          "https://www.linkedin.com/in/utshav-pandey-9b00a4190/",
          "_blank"
        );
      } else {
        window.open("https://twitter.com/utsav44", "_blank");
      }
    },
  },
};
</script>

<style lang="scss" scoped>
@import "../scss/_base.scss";
.nav-container {
  background-color: #0b4fa9;
  header {
    display: flex;
    justify-content: space-between;
    padding: 2rem;
    @include respond(phone) {
      padding: 1rem 0.8rem 1rem 1rem;
    }
  }
  &--logo {
    color: #5aff7f;
    font-size: 1.2rem;
    text-decoration: none;
    @include respond(phone) {
      font-size: 0.8rem;
      margin-left: 0rem;
    }
  }
  &--item {
    color: #dba6e3;
    font-size: 1.1rem;
    text-decoration: none;
    @include respond(phone) {
      font-size: 0.8rem;
    }
  }
  nav {
    float: right;
    ul {
      display: flex;
      a {
        display: block;
        text-decoration: none;
        padding: 0 1rem;
      }
    }
  }
}
.social-header {
  display: none;
}
.logo {
  &--navIcon {
    // height: 10%;
    width: 40%;
  }
  &--navIcon {
    // height: 10%;
    width: 100%;
  }
  &--navIcon {
    // height: 10%;
    width: 40%;
  }
}
@media only screen and (min-width: 1050px) {
  .nav-container {
    display: grid;
    grid-template-columns: 66% auto;
    background: unset;
    header {
      background: #0b4fa9;
      padding: 2em 2em 2em 4em;
    }
  }

  // .social-header {
  // padding: 0 5rem 0 2rem;
  // padding: auto;
  // align-items: center;

  // justify-content: space-around;
  // }
  .social-header {
    display: block;
    // background-color: violet;
    width: 90%;
    margin: auto auto auto auto;
    ul {
      display: flex;
      justify-content: space-evenly;
      li {
        a {
          img {
            width: 1.5rem;
          }
          .Twitter {
            width: 1.7rem;
          }
        }
      }
      // float: right;
    }
  }
}

@media only screen and (min-width: 1250px) {
  header {
    padding: 2em 2em 2em 10em;
  }
  .social-header {
    width: 60%;
    padding: 0;
    // padding: auto;
    align-items: center;
    margin: auto;
    justify-content: space-around;
    // padding: 2em 10em 2em 0;
  }
}
</style>