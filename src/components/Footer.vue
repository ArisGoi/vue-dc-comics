<template>
  <footer>
    <section class="footer-top">
      <img src="../assets/img/dc-logo-bg.png" alt="">
      <div class="container">
        <!-- DC COMICS -->
        <ul>
          <li>DC Comics</li>
          <li>Characters</li>
          <li>Comics</li>
          <li>Movies</li>
          <li>TV</li>
          <li>Games</li>
          <li>Videos</li>
          <li>News</li>
        </ul>

        <!-- SHOPS -->
        <ul>
          <li>Shop</li>
          <li>Shop DC</li>
          <li>Shop DC Collectibles</li>
        </ul>

        <!-- DC -->
        <ul>
          <li>DC</li>
          <li>Terms Of Use</li>
          <li>Privacy policy (New)</li>
          <li>Ad Choises</li>
          <li>Advertising</li>
          <li>Jobs</li>
          <li>Subscriptions</li>
          <li>Talent Workshops</li>
          <li>CPSC Certificates</li>
          <li>Ratings</li>
          <li>Shop Help</li>
          <li>Contact Us</li>
        </ul>

        <!-- Sites -->
        <ul>
          <li>Sites</li>
          <li>DC</li>
          <li>MAD Magazine</li>
          <li>DC Kids</li>
          <li>DC Universe</li>
          <li>DC Power Visa</li>
        </ul>

      </div>
    </section>
    <section class="footer-bottom">
      <div class="container">
        <button class="btn type-1">Sign-Up Now!</button>
        <ul>
          <li>Follow Us</li>
          <li><a href="#"><img src="../assets/img/footer-facebook.png" alt=""></a></li>
          <li><a href="#"><img src="../assets/img/footer-twitter.png" alt=""></a></li>
          <li><a href="#"><img src="../assets/img/footer-youtube.png" alt=""></a></li>
          <li><a href="#"><img src="../assets/img/footer-pinterest.png" alt=""></a></li>
          <li><a href="#"><img src="../assets/img/footer-periscope.png" alt=""></a></li>
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
@import '../assets/style/style.scss';

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

    .container{
      height: 100%;
      display: flex;
      align-items: flex-start;
      flex-direction: column;
      justify-content: flex-start;
      align-content: flex-start;
      flex-wrap: wrap;
    }

    ul{
      list-style: none;
      margin-top: 20px;
      margin-right: 60px;

      li{
        font-size: 1.2rem;
        color: lightslategray;

        &:first-child{
          text-transform: uppercase;
          font-size: 1.55rem;
          font-weight: 700;
          margin-bottom: .225rem;
          color: white;
        }
      }
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
