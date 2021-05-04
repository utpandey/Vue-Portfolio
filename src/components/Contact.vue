<template>
  <div class="cont">
    <div class="cont__footer">
      <div class="cont__footer__btn" @click="homeBtn">
        <svg
          class="cont__footer__btn--svg"
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M12 6L12.6508 5.24074L12 4.68292L11.3492 5.24074L12 6ZM19.6508 11.2407L12.6508 5.24074L11.3492 6.75926L18.3492 12.7593L19.6508 11.2407ZM11.3492 5.24074L4.34921 11.2407L5.65079 12.7593L12.6508 6.75926L11.3492 5.24074Z"
            fill="#CCD2E3"
          />
          <path
            d="M12 12L12.6508 11.2407L12 10.6829L11.3492 11.2407L12 12ZM19.6508 17.2407L12.6508 11.2407L11.3492 12.7593L18.3492 18.7593L19.6508 17.2407ZM11.3492 11.2407L4.34921 17.2407L5.65079 18.7593L12.6508 12.7593L11.3492 11.2407Z"
            fill="#CCD2E3"
          />
        </svg>
      </div>
      <div class="cont__footer__icons">
        <ul>
          <li>
            <a href="" @click="openProfile(1)">
              <svg
                width="30"
                height="28"
                viewBox="0 0 30 28"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                class="logo--nav"
              >
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M15 0C6.7125 0 0 6.265 0 14C0 20.195 4.29375 25.4275 10.2562 27.2825C11.0062 27.405 11.2875 26.985 11.2875 26.6175C11.2875 26.285 11.2688 25.1825 11.2688 24.01C7.5 24.6575 6.525 23.1525 6.225 22.365C6.05625 21.9625 5.325 20.72 4.6875 20.3875C4.1625 20.125 3.4125 19.4775 4.66875 19.46C5.85 19.4425 6.69375 20.475 6.975 20.895C8.325 23.0125 10.4813 22.4175 11.3438 22.05C11.475 21.14 11.8687 20.5275 12.3 20.1775C8.9625 19.8275 5.475 18.62 5.475 13.265C5.475 11.7425 6.05625 10.4825 7.0125 9.5025C6.8625 9.1525 6.3375 7.7175 7.1625 5.7925C7.1625 5.7925 8.41875 5.425 11.2875 7.2275C12.4875 6.9125 13.7625 6.755 15.0375 6.755C16.3125 6.755 17.5875 6.9125 18.7875 7.2275C21.6562 5.4075 22.9125 5.7925 22.9125 5.7925C23.7375 7.7175 23.2125 9.1525 23.0625 9.5025C24.0188 10.4825 24.6 11.725 24.6 13.265C24.6 18.6375 21.0938 19.8275 17.7563 20.1775C18.3 20.615 18.7688 21.455 18.7688 22.7675C18.7688 24.64 18.75 26.145 18.75 26.6175C18.75 26.985 19.0312 27.4225 19.7812 27.2825C25.7063 25.4275 30 20.1775 30 14C30 6.265 23.2875 0 15 0Z"
                  fill="white"
                />
              </svg>

              <!-- <img
                src="../assets/icons/github.svg"
                alt="Github"
                class="logo--nav--git"
            /> -->
            </a>
          </li>
          <li>
            <a href="" @click="openProfile(2)">
              <svg
                width="30"
                height="32"
                viewBox="0 0 30 32"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                class="logo--nav"
              >
                <path
                  d="M27.7793 0H2.21484C0.990234 0 0 1.03125 0 2.30625V29.6875C0 30.9625 0.990234 32 2.21484 32H27.7793C29.0039 32 30 30.9625 30 29.6938V2.30625C30 1.03125 29.0039 0 27.7793 0ZM8.90039 27.2687H4.44727V11.9937H8.90039V27.2687ZM6.67383 9.9125C5.24414 9.9125 4.08984 8.68125 4.08984 7.1625C4.08984 5.64375 5.24414 4.4125 6.67383 4.4125C8.09766 4.4125 9.25195 5.64375 9.25195 7.1625C9.25195 8.675 8.09766 9.9125 6.67383 9.9125ZM25.5645 27.2687H21.1172V19.8438C21.1172 18.075 21.0879 15.7937 18.8027 15.7937C16.4883 15.7937 16.1367 17.725 16.1367 19.7188V27.2687H11.6953V11.9937H15.9609V14.0813H16.0195C16.6113 12.8813 18.0645 11.6125 20.2266 11.6125C24.7324 11.6125 25.5645 14.775 25.5645 18.8875V27.2687Z"
                  fill="#fff"
                />
              </svg>

              <!-- <img
                src="../assets/icons/linkedin.svg"
                alt="Linkedin"
                class="logo--nav--link"
            /> -->
            </a>
          </li>
          <li>
            <a href="" @click="openProfile(3)">
              <svg
                width="27"
                height="23"
                viewBox="0 0 27 23"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                class="logo--nav"
              >
                <path
                  d="M8.49392 22.4688C18.6801 22.4688 24.2531 14.0277 24.2531 6.7097C24.2531 6.47238 24.2478 6.22983 24.2372 5.99251C25.3214 5.2085 26.2569 4.2374 27 3.1248C25.9903 3.57402 24.9184 3.86738 23.8206 3.9949C24.9765 3.30212 25.8419 2.21375 26.2564 0.931578C25.1691 1.57597 23.98 2.03053 22.7401 2.27578C21.9047 1.3881 20.8001 0.800347 19.5972 0.603399C18.3942 0.406451 17.1599 0.611274 16.085 1.1862C15.0101 1.76113 14.1545 2.67414 13.6506 3.78408C13.1466 4.894 13.0224 6.13904 13.297 7.3267C11.0953 7.21617 8.94144 6.64428 6.975 5.64798C5.00853 4.65162 3.27341 3.25321 1.88209 1.5433C1.17495 2.76249 0.958562 4.20522 1.27691 5.57817C1.59526 6.95118 2.42445 8.1515 3.59596 8.93506C2.71646 8.90716 1.85622 8.67035 1.08633 8.24425V8.31282C1.08554 9.59228 1.52786 10.8325 2.3381 11.8227C3.14833 12.8129 4.27649 13.492 5.53078 13.7444C4.71606 13.9674 3.86098 13.9999 3.0317 13.8394C3.38564 14.9397 4.07427 15.9021 5.00149 16.5922C5.92869 17.2823 7.04824 17.6658 8.20389 17.689C6.24195 19.2301 3.81845 20.066 1.32364 20.062C0.881196 20.0614 0.439199 20.0343 0 19.9808C2.53446 21.6068 5.48272 22.4704 8.49392 22.4688Z"
                  fill="white"
                />
              </svg>

              <!-- <img
                src="../assets/icons/twitter.svg"
                alt="Twitter"
                class="logo--nav--twit"
            /> -->
            </a>
          </li>
        </ul>
      </div>
      <div class="cont__footer__info">
        <p>Made in Vuejs per Utsav Pandey</p>
      </div>
    </div>
  </div>
</template>

<script>
import { gsap } from "gsap";
export default {
  mounted() {
    // var exit = document.querySelector(".cont__footer__btn");
    // var offset = document.getElementById("#homePage").
    // exit.addEventListener("click", () => {
    //   TweenLite.to(window, 1, { scrollTo: { y: offset } });
    // });
    // var offset = document.getElementById("#homePage");
    // // offset().top;
    // var exit = document.querySelector(".cont__footer__btn");
    // exit.addEventListener("click", () => {
    //   console.log("sadsadsad");
    //   TweenLite.to(window, 1, { scrollTo: { y: offset } });
    // });
  },
  // data() {},
  methods: {
    homeBtn() {
      var t1 = gsap.timeline();
      t1.to(".hero", {
        duration: 1.2,
        width: "100%",
        ease: "Expo.easeInOut",
      });
      console.log("sadsadsad");
    },
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
    // f
  },
};
</script>

<style lang="scss" scoped>
@import "../scss/_base.scss";
.right {
  float: right;
}
.cont {
  text-align: center;
  height: 100%;
  background-color: #e5e5e5;
  // margin: -2rem 0 0 0;
  // padding-top: 3rem;
  // padding: 2rem 0 2rem 0;
  &__body {
    position: relative;
    padding: 5rem;
    // text-align: center;
    // justify-items: center;
    // align-items: center;
    // justify-content: center;
    // z-index: -1;
    svg {
      position: absolute;
      top: 2rem;
      left: 2rem;
    }
  }
  &__footer {
    background-color: #838080;
    // text-align: center;
    // height: 100%;
    position: relative;
    &__btn {
      cursor: pointer;
      background-color: rgb(243, 6, 6);
      height: 40px;
      width: 40px;
      position: absolute;
      left: 50%;
      top: 0%;
      transform: translate(-50%, -50%);
      border-radius: 50%;
      // @include respond(phone) {
      //   margin-left: 46%;
      // }
      &--svg {
        cursor: pointer;
        margin-top: 0.4rem;
      }
    }
    &__icons {
      padding-top: 10rem;
      position: relative;
      ul {
        display: flex;
        position: absolute;
        left: 50%;
        top: 50%;
        transform: translate(-50%, -50%);
      }
      .logo--nav {
        padding: 2rem 2rem 0 2rem;
      }
      // ul {
      //   background-color: violet;
      //   display: flex;
      //   list-style: none;
      //   padding-left: 0;
      //   float: left;
      //   margin-top: 15px;
      //   margin-right: 50px;
      //   // justify-content: space-evenly;
      //   a {
      //     display: block;
      //     // margin: 2rem 0 0 6rem;
      //     padding: 2rem 0 0rem 0;
      //   }
      // }
    }
    &__info {
      padding-bottom: 2rem;
      p {
        font-weight: bold;
        color: white;
      }
    }
  }
  h1 {
    font-family: "Poppins", sans-serif, "arial";
    font-weight: 600;
    // font-size: 72px;
    // color: white;
    // text-align: center;
  }

  h4 {
    font-family: "Roboto", sans-serif, "arial";
    font-weight: 400;
    font-size: 20px;
    color: #9b9b9b;
    line-height: 1.5;
  }

  /* ///// inputs /////*/

  input:focus ~ label,
  textarea:focus ~ label,
  input:valid ~ label,
  textarea:valid ~ label {
    font-size: 0.75em;
    color: #999;
    top: -5px;
    -webkit-transition: all 0.225s ease;
    transition: all 0.225s ease;
  }

  .styled-input {
    float: left;
    width: 293px;
    margin: 1rem 0;
    position: relative;
    border-radius: 4px;
  }

  @media only screen and (max-width: 768px) {
    .styled-input {
      width: 100%;
    }
  }

  .styled-input label {
    color: #999;
    padding: 1.3rem 30px 1rem 30px;
    position: absolute;
    top: 10px;
    left: 0;
    -webkit-transition: all 0.25s ease;
    transition: all 0.25s ease;
    pointer-events: none;
  }

  .styled-input.wide {
    width: 650px;
    max-width: 100%;
  }

  input,
  textarea {
    padding: 30px;
    border: 0;
    width: 100%;
    font-size: 1rem;
    background-color: #2d2d2d;
    color: white;
    border-radius: 4px;
  }

  input:focus,
  textarea:focus {
    outline: 0;
  }

  input:focus ~ span,
  textarea:focus ~ span {
    width: 100%;
    -webkit-transition: all 0.075s ease;
    transition: all 0.075s ease;
  }

  textarea {
    width: 100%;
    min-height: 15em;
  }

  .input-container {
    width: 650px;
    height: 500px;
    max-width: 100%;
    margin: 2rem auto 25px auto;
    @include respond(phone) {
      height: 700px;
      margin: 2rem 0 0 -2rem;
    }
  }

  .submit-btn {
    padding: 7px 35px;
    border-radius: 2%;
    display: inline-block;
    background-color: #0f0f0f;
    color: white;
    font-size: 18px;
    cursor: pointer;
    box-shadow: 0 2px 5px 0 rgba(0, 0, 0, 0.06),
      0 2px 10px 0 rgba(0, 0, 0, 0.07);
    -webkit-transition: all 300ms ease;
    transition: all 300ms ease;
  }

  .submit-btn:hover {
    transform: translateY(1px);
    box-shadow: 0 1px 1px 0 rgba(0, 0, 0, 0.1), 0 1px 1px 0 rgba(0, 0, 0, 0.09);
  }

  .error-message {
    color: rgb(177, 18, 18);
  }

  .success-message {
    color: green;
  }

  @media (max-width: 768px) {
    .submit-btn {
      width: 97%;
      float: none;
      text-align: center;
    }
  }

  input[type="checkbox"] + label {
    color: #ccc;
    font-style: italic;
  }

  input[type="checkbox"]:checked + label {
    color: #f00;
    font-style: normal;
  }
}
</style>
<!--
 <div class="cont__body">
      <svg
        width="76"
        height="60"
        viewBox="0 0 76 60"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M3.42893 3.76218C0.5 6.69112 0.5 11.4052 0.5 20.8332V39.1666C0.5 48.5947 0.5 53.3087 3.42893 56.2377C6.35786 59.1666 11.0719 59.1666 20.5 59.1666H55.5C64.9281 59.1666 69.6421 59.1666 72.5711 56.2377C75.5 53.3087 75.5 48.5947 75.5 39.1666V20.8333C75.5 11.4052 75.5 6.69112 72.5711 3.76218C69.6421 0.833252 64.9281 0.833252 55.5 0.833252H20.5C11.0719 0.833252 6.35786 0.833252 3.42893 3.76218ZM13.5547 16.6679C13.0952 16.3615 12.4743 16.4857 12.1679 16.9452C11.8616 17.4047 11.9858 18.0256 12.4453 18.332L36.8906 34.6288C37.5624 35.0767 38.4376 35.0767 39.1094 34.6288L63.5547 18.332C64.0142 18.0256 64.1384 17.4047 63.8321 16.9452C63.5257 16.4857 62.9048 16.3615 62.4453 16.6679C47.6424 26.5365 28.3576 26.5365 13.5547 16.6679Z"
          fill="white"
        />
      </svg>

       <div className="row">
        <h1>Contact Form</h1>
      </div> 
      <div className="row input-container">
        <div className="col-md-6 col-sm-12">
          <div className="styled-input">
            <input type="text" required />
            <label>Name</label>
          </div>
        </div>
        <div className="col-md-6 col-sm-12 right">
          <div className="styled-input">
            <input type="text" required />
            <label>Email</label>
          </div>
        </div>
        <div className="col-md-6 col-sm-12">
        style={{ float: 'right' }} 
          <div className="styled-input">
            <input type="text" required />
            <label>Subject</label>
          </div>
        </div>
        <div className="col-xs-12">
          <div className="styled-input wide">
            <textarea value="" required />
            <label>Text</label>
            {error ? <p className="error-message ">{error}</p> : null}
						{success ? <p className="success-message ">{success}</p> : null} 
          </div>
        </div>
        <div className="col-xs-12">
          <div className="btn-lrg submit-btn">Send Message</div>
        </div>
      </div>
    </div>-->