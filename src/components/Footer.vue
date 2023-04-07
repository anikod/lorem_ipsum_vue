<script>
// import i1 from '../assets/icons/i-1.svg';
</script>


<template>
  <div class="footer">

    <p>&copy 2018 &laquo;LOREMIPSUM.NET&raquo; Все права <br> защищены.</p>

    <img src="../assets/icons/vertical.svg" alt="">


    <div class="footer__item footer__item_qiwi">QIWI wallet</div>
    <div class="footer__item footer__item_ym">Yandex Money</div>
    <div class="footer__item footer__item_wm">Web Money</div>

    <img src="../assets/icons/vertical.svg" alt="">

    <a href="mailto:info@ipsum228.com" class="footer__link"><div class="footer__item footer__item_mail">info@ipsum228.com</div></a>

    <a href="https://vk.com" class="footer__link"><div class="footer__item footer__item_vk">Мы вконтакте</div></a>

  </div>
</template>


<style lang="scss">
.footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: white;
  font-size: 0.8rem;
  padding-top: 15px;
  // padding: 0;
  margin: 0;
  // border: 1px solid red;

  &__item {
    font-weight: normal;
    // margin: 0 auto;
    text-align: center;
    flex: 0 1 8%;
    position: relative;
    // border: 41x solid red;

    &_qiwi::before {
      content: "";
      position: absolute;
      left: -15px;
      top: -3px;
      background-image: url('../assets/icons/qiwi.svg');
      background-repeat: no-repeat;
      width: 100px;
      height: 50px;
    }

    &_ym::before {
      content: "";
      position: absolute;
      left: -20px;
      top: -5px;
      background-image: url('../assets/icons/ym.svg');
      background-repeat: no-repeat;
      width: 100px;
      height: 50px;
    }

    &_wm::before {
      content: "";
      position: absolute;
      left: -20px;
      top: -5px;
      background-image: url('../assets/icons/wm.svg');
      background-repeat: no-repeat;
      width: 100px;
      height: 50px;
    }

    &_mail::before {
      content: "";
      position: absolute;
      left: -30px;
      top: 2px;
      background-image: url('../assets/icons/mail.svg');
      background-repeat: no-repeat;
      width: 100px;
      height: 50px;
    }

    &_vk::before {
      content: "";
      position: absolute;
      left: -20px;
      top: -0px;
      background-image: url('../assets/icons/vk.svg');
      background-repeat: no-repeat;
      width: 100px;
      height: 50px;
    }

    
  }
}

a.footer__link, a.footer__link:link, a.footer__link:visited, a.footer__link a:active {
  color: white;
}

@media (max-width: 320px) {
  $bgcolor: none;

  $color: teal;

}
</style>