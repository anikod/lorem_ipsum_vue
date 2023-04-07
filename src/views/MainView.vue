<script setup>
// import TheWelcome from '../components/TheWelcome.vue'
import 'normalize.css';
import Header from '../components/Header.vue';
import Picture from '../components/Picture.vue';
import Order from '../components/Order.vue';
import Footer from '../components/Footer.vue';

// app.component('#3E9CDC', textblue);
</script>


<template>
  <div class="wrapper bgimage">

    <div class="section section-header">
      <div class="container">
        <section>
          <Header />
        </section>
      </div>
    </div>

    <div class="section">
      <div class="section-picture">
        <div class="container">
          <section>
            <Picture />
          </section>
        </div>
      </div>
    </div>

    <div class="section section-order">
      <div class="container">
        <main>
          <section>
            <Order />
          </section>
        </main>
      </div>
    </div>


    <div class="section section-footer">

      <div class="container">
        <footer>
          <Footer />
        </footer>
      </div>
    </div>

  </div>
</template>


<style lang="scss">
// $textblue: #3E9CDC;

@font-face {
  font-family: "Lato";
  src: local("Lato"),
    url(@/assets/fonts/Lato/Lato-Regular.ttf) format("truetype");
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: "Lato";
  src: local("Lato"),
    url(@/assets/fonts/Lato/Lato-Bold.ttf) format("truetype");
  font-weight: bold;
  font-style: normal;
}

@font-face {
  font-family: "Lato";
  src: local("Lato"),
    url(@/assets/fonts/Lato/Lato-Black.ttf) format("truetype");
  font-weight: 900;
  font-style: normal;
}

body,
* {
  font-family: "Lato", sans-serif, monospace;
  // color: $textblue;
}

.wrapper {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  margin: 0;
  padding: 0;
  // width: 100vw;
  // margin: 0 auto;
  min-height: 100vh;
  // object-fit: cover;
  max-width: 1920px;
  margin: 0 auto;
  box-sizing: border-box;

}

.section {
  // box-sizing: border-box;
  // flex: 1 0 1920px;
  // max-width: 100vw;
  // max-width: 1920px;
  // flex: 0 0 auto;
  // flex-basis: 1920px;
  // border: 5px solid red;
  // display: flex;
  // flex-direction: row;
  // margin: 0;
  // padding: 0;
  width: 100vw;
  max-width: 1920px;
  // margin: 0 auto;

  &-header {
    // flex: 1 1 1920px;
    // border: 4px solid yellow;
    position: fixed;
    background-color: rgba(16, 16, 29, 0.9);
  }

  &-picture {
    font-weight: normal;
  }

  &-order {
    flex: 0 0 915px;
    background-color: rgba(16, 16, 29, 0.9);
    // background-image: url('/public/order-bg.webp');
    background-image: url('../assets/order-bg.webp');
  }

  &-footer {
    flex: 0 0 90px;
    // padding: 10px;
    background-color: rgb(61, 64, 80);
  }
}

.bgimage {
  background-image: url('../assets/header.webp');
  // position: relative;
  background-repeat: no-repeat;
  background-position: center top;
}



.container {
  max-width: 1172px;
  margin: 0 auto;
}

@media (max-width: 320px) {
  $bgcolor: none;


}
</style>