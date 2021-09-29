<template>
  <footer>
    <section class="footer-top">
      <img src="@/assets/img/dc-logo-bg.png" alt="">
      <div class="container">
        TEXT
      </div>
    </section>
    <section class="footer-bottom">
      <div class="container">
        <button>Sign-Up Now</button>
        <ul>
          <li>Follow Us</li>
          <li><a href="#"><img src="@/assets/img/footer-facebook.png" alt=""></a></li>
          <li><a href="#"><img src="@/assets/img/footer-twitter.png" alt=""></a></li>
          <li><a href="#"><img src="@/assets/img/footer-youtube.png" alt=""></a></li>
          <li><a href="#"><img src="@/assets/img/footer-pinterest.png" alt=""></a></li>
          <li><a href="#"><img src="@/assets/img/footer-periscope.png" alt=""></a></li>
        </ul>
      </div>
    </section>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
}
</script>

<!-- Style SCSS -->
<style scoped lang="scss">
@import '@/assets/style/style.scss';

  .footer-top{
    height: 370px;
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    position: relative;
    overflow: hidden;

    img{
      position: absolute;
      top: 50%;
      transform: translateY(-50%);
      right: 50px;
    }
  }

  .footer-bottom{
    height: 6.25rem;
    background-color: $c-footer;

    .container{
      height: 100%;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    
    ul{
      display: flex;
      align-items: center;
      li{
        display: inline-block;
        color: $c-first;
        text-transform: uppercase;
        font-weight: 700;

        a{
          padding: 10px;
        }
      }
    }
  }
</style>
