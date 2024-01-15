<template>
  <div class="header">
    <div className="header_container">
      <a href="/" className="header__logo">
        <img src="../assets/logo.svg" alt="logo" />
      </a>

      <nav v-if="isWideScreen" class="desktop-menu header__nav">
        <ul className="header__nav-ul">
          <li className="header__nav-list">
            <a className="header__nav-link" href="/"> Features </a>
          </li>
          <li className="header__nav-list">
            <a className="header__nav-link" href="/"> Pricing </a>
          </li>
          <li className="header__nav-list">
            <a className="header__nav-link" href="/"> Blog </a>
          </li>
          <li className="header__nav-list">
            <a className="header__nav-link" href="/"> Docs </a>
          </li>
          <li className="header__nav-list">
            <a className="header__nav-link" href="/"> Changelog </a>
          </li>
          <li className="header__nav-list">
            <a className="header__nav-link" href="/"> We're hiring </a>
          </li>
        </ul>
        <button className="btn header__btn">Login</button>
      </nav>

      <div v-else>
        <button @click="toggleMenu" class="burger-button">
          <span class="burger-line"></span>
          <span class="burger-line"></span>
          <span class="burger-line"></span>
        </button>
        <div v-if="isMenuOpen" class="menu">
          <!--  burger menu  -->
          <a href="#">Home</a>
          <a href="#">About</a>
          <a href="#">Services</a>
          <a href="#">Contact</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// import { ref, onMounted, onUnmounted } from 'vue';

export default {
  data() {
    return {
      isMenuOpen: false,
      isWideScreen: window.innerWidth >= 1000,
    };
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    },
    handleResize() {
      this.isWideScreen = window.innerWidth >= 1000;
    },
  },
  mounted() {
    window.addEventListener("resize", this.handleResize);
  },
  beforeUnmount() {
    window.removeEventListener("resize", this.handleResize);
  },
};
</script>

<style scoped lang="scss">
.header {
  &_container {
    display: flex;
    justify-content: space-between;
    padding: 20px 16px;
    align-items: center;
  }

  &__btn {
    padding: 6px 22px;
    border-radius: 12px;
    background: $black;
    color: $white;
    font-size: 14px;
    font-weight: 400;
    line-height: 20px;

    transition: 0.7s;

    &:hover{
      color:black;
      background: white;
  }
}

  &__nav {
    display: contents;
    &-ul {
      display: flex;
      gap: 48px;
    }
    &-link {
      color: $text-color;
      transition: 0.4s;

      &:hover{
      color: rgb(255, 183, 0);
      

    }
    }
  }

  .burger-button {
    background: none;
    border: none;
    cursor: pointer;
  }

  .burger-line {
    display: block;
    width: 25px;
    height: 3px;
    background-color: #333;
    margin: 5px 0;
  }

  .menu {
    display: flex;
    // flex-direction: column;

    position: absolute;

    flex-direction: row;
    right: 10px;
    gap: 30px;
    background: aliceblue;
    border: 16px;
    border: 2px solid;
    border-radius: 16px;

    @media only screen and (max-width: 425px) {
      top: 11%;
    gap: 24px;
  }
  }

  .menu a {
    text-decoration: none;
    color: #333;
    padding: 5px;
    margin: 5px 0;
  }
}
</style>
