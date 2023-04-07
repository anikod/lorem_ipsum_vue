<script>
// import i1 from '../assets/icons/i-1.svg';
</script>


<template>
  <div class="order">

    <!-- <div class="content"> -->
    <h2>Оформление <span>заказа</span></h2>

    <h4>Перед заполнением формы ознакомьтесь с нашей схемой работы!</h4>

    <div class="howtoorder">
      <div class="howtoorder__item">
        <img src="../assets/icons/i-1.svg" alt="" width="100" height="100">
        <p>Lorem ipsum dolor sit amet</p>
      </div>

      <div class="howtoorder__item">
        <img src="../assets/icons/i-2.svg" alt="" width="100" height="100">
        <p>Сonsecteturadipiscing elit</p>
      </div>

      <div class="howtoorder__item">
        <img src="../assets/icons/i-3.svg" alt="" width="100" height="100">
        <p>Sed do eiusmod tempor</p>
      </div>

      <div class="howtoorder__item">
        <img src="../assets/icons/i-4.svg" alt="" width="100" height="100">
        <p>Esse cillum dolore eu fugiat</p>
      </div>

      <div class="howtoorder__item">
        <img src="../assets/icons/i-5.svg" alt="" width="100" height="100">
        <p>Excepteur sint occaecat cupidatat <wbr> non proident</p>
      </div>
    </div>



    <div class="order-form">
      <form action="#">

        <select>
          <option disabled>Выберите тип системы</option>
          <option value="1">Sed ut perspiciatis</option>
          <option value="2">Nemo enim ipsam</option>
          <option value="3">Et harum quidem</option>
          <option value="4">Temporibus autem</option>
          <option value="5">Itaque earum rerum</option>
        </select>

        <input type="email" value="Ваш e-mail" name="">

        <input type="text" value="Ваше имя">
        <br>

        <input type="range" class="ranged">

        <label class="input-file">
          <input type="file" name="file">
        </label>
        <br>

        <input type="button" value="Прикрепить файл">
        
        <input type="submit" value="Отправить">
      </form>
    </div>


  </div>
</template>


<style lang="scss">
$textblue: #3E9CDC;

 // передрано для кнопки отправки файла
 .input-file {
	position: relative;
	display: inline-block;
}
.input-file-btn {
	position: relative;
	display: inline-block;
	cursor: pointer;
	outline: none;
	text-decoration: none;
	font-size: 14px;
	vertical-align: middle;
	color: rgb(255 255 255);
	text-align: center;
	border-radius: 4px;
	background-color: #419152;
	line-height: 22px;
	height: 40px;
	padding: 10px 20px;
	box-sizing: border-box;
	border: none;
	margin: 0;
	transition: background-color 0.2s;
}
.input-file-text {
	padding: 0 10px;
	line-height: 40px;
	display: inline-block;
}
.input-file input[type=file] {
	position: absolute;
	z-index: -1;
	opacity: 0;
	display: block;
	width: 0;
	height: 0;
}

  // /передрано


.order-form {
  margin-top: 50px;
  font-family: sans-serif;
  font-size: 1rem;

 

  & input {
    height: 45px;
    width: 350px;
    margin: 20px;
  }

  & .ranged {
    width: 760px;
  }

  & select {
    background-color: black;
    height: 45px;
    width: 350px;
  }
}


.howtoorder {
  margin-top: 60px;
  display: flex;
  justify-content: center;
  // align-items: baseline;
  // border: 1px solid red;
  width: 1170px;

  &__item {
    // border: 1px solid red;
    font-weight: normal;
    margin: 0 auto;
    text-align: center;
    flex: 0 1 20%;
    position: relative;
    // border: 41x solid red;
  }

  &__item::after {
    content: "";
    position: absolute;
    left: 180px;
    top: 50px;
    background-image: url('../assets/dots5.svg');
    background-repeat: no-repeat;
    width: 120px;
    height: 100px;
  }

  &__item:last-child::after {
    display: none;
  }

}

.order {
  display: flex;
  flex-direction: column;
  align-items: center;
  // flex-basis: 915px;
  justify-content: center;
  color: white;
}

h2 {
  color: white;
  text-transform: uppercase;
  font-size: 2.25rem;
  margin-top: 120px;
  margin-bottom: 10px;

  & span {
    color: $textblue;
  }
}

h4 {
  color: white;
  font-weight: normal;
  letter-spacing: 0.07rem;
  ;
}






@media (max-width: 320px) {
  $bgcolor: none;

  $color: teal;

}
</style>