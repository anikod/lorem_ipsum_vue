<script>

</script>


<template>
  <div class="header">

    <div class="logo">
      <img src="@/assets/logo.png" alt="LoremIpsum.Net">
    </div>

    <nav class="header-menu">
      <ul class="header-menu__list">
        <li class="header-menu__item"><a href="#" class="header-menu__link">Бизнес</a></li>
        <li class="header-menu__item"><a href="#" class="header-menu__link">О нас</a></li>
        <li class="header-menu__item"><a href="#" class="header-menu__link">Цены</a></li>
        <li class="header-menu__item"><a href="#" class="header-menu__link">Оформить заказ</a></li>
      </ul>
    </nav>
  </div>
</template>


<style lang="scss">
$textblue: #3E9CDC;

// $color: teal;

.header {
  margin: 0;
  padding: 0;
  // background-color: rgba(16, 16, 29, 0.9);
  // padding: 5px;
  transition: all 0.5s;
  height: 100px;
  // max-width: 1920px;
  // position: fixed;
  // width: 1920px;
  // max-width: 1920px;
  // display: flex;
  // width: 1920px;
  // flex: 1 1 auto;
  // display: flex;
  // flex-direction: row;
  // justify-content: space-between;
  // border: 5px solid red;

}


.logo {
  color: white;
  display: inline;
  // font-size: 2rem;
  // height: 100px;
  line-height: 100px;
  margin-left: 5px;
  // border: 1px solid red;
  // vertical-align: middle;

  // flex: 0 0 400px;

  & img {
    vertical-align: middle;
  }

}


.header-menu {
  width: 450px;
  float: right;

  &__list {
    // border: 1px solid $color;
    height: 100px;
    // vertical-align: middle;
    // border: 1px solid red;
    margin: 0;
    padding: 0;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    // width: 400px;
    // height: 100px;

  }

  &__item,
  &__item li {
    // flex: 0 0 120px;
    list-style: none;
    // display: inline-block;
    // flex-basis: 500px;
    // flex: 1 1 auto;
    // text-align: center;

  }

  &__link {
    // border: 1px solid red;
    // line-height: 100px;
    padding: 1.2rem;
    overflow: hidden;

    color: white;
    font-size: 0.75rem;
    font-weight: normal;
    text-transform: uppercase;
    text-decoration: none;
    transition: all 0.25s ease;
  }

  &__link:hover {
    text-decoration: underline;
    color: $textblue;
  }

  &__item:last-child a {
    // font-size: 3rem;
    padding-right: 0;
    // margin: 0;
    // border: 1px solid red;
    letter-spacing: 0.07rem;
    ;
  }
}

@media (max-width: 320px) {}
</style>