<template>
  <section>
    <div class="container">
      <ul>
        <li>
          <img src="@/assets/img/buy-comics-digital-comics.png" alt="">
          <h4>Digital Comics</h4>
        </li>
        <li>
          <img src="@/assets/img/buy-comics-merchandise.png" alt="">
          <h4>Digital Comics</h4>
        </li>
        <li>
          <img src="@/assets/img/buy-comics-subscriptions.png" alt="">
          <h4>Digital Comics</h4>
        </li>
        <li>
          <img src="@/assets/img/buy-comics-shop-locator.png" alt="">
          <h4>Digital Comics</h4>
        </li>
        <li>
          <img src="@/assets/img/buy-dc-power-visa.svg" class="svg" alt="">
          <h4>Digital Comics</h4>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: 'dcIndexBar',
}
</script>

<!-- Style SCSS -->
<style scoped lang="scss">
@import '@/assets/style/style.scss';

  section{
    background-color: $c-first;
    width: 100%;
  }

  ul{
    display: flex;
    justify-content: space-around;
    align-items: center;
    height: 100px;
  }

  li{
    list-style: none;
    display: flex;
    align-items: center;

    img{
      height: 3rem;
    }
    img.svg{
      height: 2.5rem;
    }

    h4{
      font-size: 1.25rem;
      margin-left: .5125rem;
      color: white;
    }
  }
</style>
