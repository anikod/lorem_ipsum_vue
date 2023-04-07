<script>
// import bgimage from '../assets/header_src-min.jpg';
// import Header from '/src/components/Header.vue'
</script>


<template>
  <!-- <img src="/public/header.webp" alt="" /> -->
  <div class="picture">

    <article class="picture__content">
      <h1><span>LOREM IPSUM</span> DOLOR SIT <br>
        amet consectetur <br>
        <span>adipiscing</span></h1>


      <h4>At vero eos et accusamus et iusto odio dignissimos ducimus!</h4>

      <ul>
        <li>Totam rem aperiam eaque ipsa</li>
        <li>Sit voluptatem accusantium doloremque laudantium</li>
        <li>Sed ut perspiciatis, unde omnis iste natus error</li>
      </ul>

      <button>Заказать</button>

      <button class="right">Подробнее</button>
    </article>


  </div>
</template>


<style lang="scss">
$textblue: #3E9CDC;

.picture {
  min-height: 850px;
  // width: 100vw;
  // flex: 1 1 auto;
  margin: 0;
  padding: 0;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;



  &__content {
    // vertical-align: middle;
    // border: 1px solid red;
    flex: 0 0 500px;
    width: 100%;
  }

  & h1 {
    font-size: 3rem;
    font-weight: bold;
    text-transform: uppercase;
    letter-spacing: 0.05rem;
  }

  & h1 span {
    // border: 1px solid red;
    color: $textblue;
    // vertical-align: middle;
  }

  & h4 {
    font-size: 1.25rem;
    font-weight: bold;
    margin: 2.25rem 0 0.66rem;
  }

  & ul {
    margin: 0;
    margin-bottom: 80px;
    padding: 0;
    font-size: 1.25rem;
  }

  & ul li {
    list-style: '-';
    margin-left: 0.9rem;
    margin-bottom: 0.4rem;
    padding-left: 1rem;
  }

button {
  width: 180px;
  height: 40px;
  margin-right: 40px;
  text-transform: uppercase;
  font-weight: normal;
  font-size: 0.80rem;
  border: 1px solid black;
  border-radius: 4px;
  transition: all 0.15s ease;
  // color: white;
  
  &:hover {
    background-color: $textblue;
    color: white;
    border: 1px solid white;
  }
}




}




</style>