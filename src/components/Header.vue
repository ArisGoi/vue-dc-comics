<template>
  <header>
    <div class="container flex-ori">
      <img class="logo" src="@/assets/img/dc-logo.png" alt="Logo DC">
      <nav>
        <ul>
          <li><a href="#">Characters</a></li>
          <li><a href="#">Comics</a></li>
          <li><a href="#">Movies</a></li>
          <li><a href="#">TV</a></li>
          <li class="current"><a href="#">Games</a></li>
          <li><a href="#">Collectibles</a></li>
          <li><a href="#">Videos</a></li>
          <li><a href="#">Fans</a></li>
          <li><a href="#">News</a></li>
          <li><a href="#">Shop</a></li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  @import '@/assets/style/style.scss';

  header{
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    background-color: $c-header;

    .container{
      justify-content: space-between;
      align-items: center;
      height: $header-height;
    }
    .logo{
      height: $header-logo-h;
    }

    nav ul{
      display: flex;

      li{
        height: $header-height;
        display: flex;
        align-items: center;
        position: relative;

        &.current a{
          color: $c-first;
        }
        &.current::after{
          content: '';
          position: absolute;
          bottom: 0;
          left: 0;

          height: 5px;
          width: 100%;
          background-color: $c-first;
        }
      }

      a{
        color: $c-text-main;
        text-decoration: none;
        font-weight: 700;
        padding: 15px;
        font-size: 18px;
      }
    }
  }
</style>
