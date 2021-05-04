<template>
  <div class="cont">
    <div class="cont__top">
      <p>Check out my blogs!</p>
    </div>
    <div class="cont__bottom">
      <div class="cont__bottom__item transition3">
        <img
          src="../assets/images/ReactJs-1.png"
          alt=""
          class="cont__bottom__item--img"
        />
        <div class="cont__bottom__item__desc">
          <p class="cont__bottom__item__desc--title">
            React.js contact form with AWS Lambda and SES to send email! (Part -
            1)
          </p>
          <p class="cont__bottom__item__desc--info">
            In this tutorial we are going to build a full-stack React app with
            AWS Server-less as the back-end.
          </p>
        </div>
      </div>
      <div class="cont__bottom__item transition3">
        <img
          src="../assets/images/ReactJs-2.png"
          alt=""
          class="cont__bottom__item--img"
        />
        <div class="cont__bottom__item__desc">
          <p class="cont__bottom__item__desc--title">
            React.js contact form with AWS Lambda and SES to send email! (Part -
            2)
          </p>
          <p class="cont__bottom__item__desc--info">
            Continuing our tutorial to create a full-stack React app with AWS
            Server-less back-end, lets jump to the terminal.
          </p>
        </div>
      </div>
      <div class="cont__bottom__item transition3">
        <img
          src="../assets/images/ReactJs-3.png"
          alt=""
          class="cont__bottom__item--img"
        />
        <div class="cont__bottom__item__desc">
          <p class="cont__bottom__item__desc--title">
            React.js contact form with AWS Lambda and SES to send email! (Part -
            3)
          </p>
          <p class="cont__bottom__item__desc--info">
            We have finally reached the last part of our full-stack app and the
            remaining part will be focused on react.js.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "../scss/_base.scss";
.cont {
  text-align: center;
  height: 100%;

  &__top {
    padding: 2rem 0 1.5rem 0;
    p {
      text-transform: uppercase;
      font-weight: bold;
      font-size: 2rem;
      letter-spacing: 0.1rem;
      @include respond(phone) {
        font-size: 1.4rem;
      }
    }
  }
  &__bottom {
    background-color: #dfc3e6;
    display: flex;
    flex-direction: row;
    padding: 4rem 1rem 0rem 1rem;
    @include respond(tab-land) {
      flex-direction: column;
      padding-bottom: 3rem;
    }
    &__item {
      &--img {
        // height: 30%;
        width: 80%;
        @include respond(tab-land) {
          width: 50%;
        }
      }
      &__desc {
        &--title {
          font-size: 1.5rem;
          @include respond(tab-land) {
            font-size: 2rem;
            padding: 0 2rem 0 2rem;
          }
          @include respond(phone) {
            font-size: 1.3rem;
          }
          @include respond(small-phone) {
            font-size: 1.1rem;
          }
        }
        &--info {
          display: none;
          font-size: 1.5rem;
          // padding: 0 3rem 0 3rem;
          @include respond(tab-land) {
            display: block;
            padding: 0 5rem 0 5rem;
          }
          @include respond(phone) {
            padding: 0 1rem 0 1rem;
            font-size: 1rem;
            color: rgb(58, 57, 57);
          }
        }
      }
    }
  }
}
.cont__bottom__item:not(:last-child) {
  padding-bottom: 3rem;
}
</style>