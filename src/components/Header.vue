<template>
  <header>
    <nav class="container flex-ori">
      <img class="logo" src="@/assets/img/dc-logo.png" alt="Logo DC">
      <ul>
        <li v-for="(link, index) in navMenu"
        :key="index"
        :class="{current : navMenu[index].current}"
        @click="setCurrent(index)"
        >
          <a :href="navMenu[index].url">
            {{navMenu[index].title}}
          </a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'Header',

  data() {
    return {
      navMenu: [
        {
          title: "Characters",
          url: '#',
          current: false
        },
        {
          title: "Comics",
          url: '#',
          current: true
        },
        {
          title: "Movies",
          url: '#',
          current: false
        },
        {
          title: "TV",
          url: '#',
          current: false
        },
        {
          title: "Games",
          url: '#',
          current: false
        },
        {
          title: "Characters",
          url: '#',
          current: false
        },
        {
          title: "Videos",
          url: '#',
          current: false
        },
        {
          title: "Fans",
          url: '#',
          current: false
        },
        {
          title: "News",
          url: '#',
          current: false
        },
        {
          title: "Shop",
          url: '#',
          current: false
        }
      ]
    }
  },
  methods: {
    setCurrent(index) {
      for(let i=0; i < this.navMenu.length; i++){
        this.navMenu[i].current = false;
      }
      this.navMenu[index].current = true;
    }
  }
}
</script>

<!-- Style SCSS -->
<style scoped lang="scss">
  @import '@/assets/style/style.scss';

  header{
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    background-color: $c-header;
    z-index: 10;

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
