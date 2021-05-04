<template>
  <div class="proj__cont">
    <div class="header">
      <p>Check out some of my projects!</p>
    </div>
    <div class="body">
      <div class="body__item">
        <div class="body__item__left transition2">
          <p class="body__item__left--title">StockFolio</p>
          <p class="body__item__left--info">
            StockFolio is a (mock) stock market picker where one can build their
            portfolio from the Nifty50 stocks. This is a React, Redux,
            Typescript project with Scss, Framer motion and Firebase.
          </p>
        </div>
        <img
          src="../assets/images/sf-2.png"
          alt=""
          class="body__item__right transition2"
        />
      </div>
      <div class="body__item">
        <div class="body__item__left transition2">
          <p class="body__item__left--title">FindMyRepo</p>
          <p class="body__item__left--info">
            This is a React + Typescript project implemented using Scss and
            Framer motion for querying a github user's profile or repository
            using the Github's GraphQL Api.
          </p>
        </div>
        <img
          src="../assets/images/fmr-1.png"
          alt=""
          class="body__item__right transition2"
        />
      </div>
      <div class="body__item">
        <div class="body__item__left transition2">
          <p class="body__item__left--title">Node todo app</p>
          <p class="body__item__left--info">
            Node todo app is a node cli app which uses lowdb to save our todos
            tasks.
          </p>
        </div>
        <img
          src="../assets/images/ntodo-1.png"
          alt=""
          class="body__item__right transition2 nodeTodo"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "../scss/_base.scss";
.proj__cont {
  text-align: center;
  height: 100%;

  .header {
    padding: 2rem 0 1.5rem 0;
    p {
      text-transform: uppercase;
      font-weight: bold;
      font-size: 2rem;
      letter-spacing: 0.1rem;
      @include respond(phone) {
        font-size: 1.3rem;
      }
      @include respond(tab-land) {
        font-size: 1.8rem;
      }
      @include respond(tab-port) {
        font-size: 1.4rem;
      }
    }
  }
  .body {
    background-color: whitesmoke;
    &__item {
      padding: 3rem 0 3rem 0;
      display: flex;
      width: 100vw;
      @include respond(tab-land) {
        flex-direction: column;
        padding: 1rem 0 1rem 0;
      }
      &__left {
        flex: 0.6;
        &--title {
          font-weight: bold;
          font-size: 2rem;
          @include respond(phone) {
            font-size: 1.6rem;
          }
        }
        &--info {
          font-size: 1.4rem;
          margin: auto;
          padding: 0 10rem 0 10rem;
          margin-bottom: 3rem;
          @include respond(phone) {
            padding: 0 1rem 0 1rem;
            font-size: 1rem;
            color: rgb(58, 57, 57);
          }
        }
      }
      &__right {
        flex: 0.4;
        // height: 50%;
        width: 40%;
        float: right;
        @include respond(tab-land) {
          width: 60%;
          margin: auto;
        }
        @include respond(phone) {
          // margin: 0rem 0 0rem 0;
          width: 70%;
        }
      }
    }
  }
}

.nodeTodo {
  // float: right;
  // width: 30% !important;
}
</style>