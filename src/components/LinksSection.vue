<template>
  <div class="links">
    <div className="links_container">
      <div class="links-colums">
        <div className="links__colm1">
          <a className="links__colm-link" href=""><span>Gitpod</span></a>
          <a className="links__colm-link" href="">Home</a>
          <a className="links__colm-link" href="">Features</a>
          <a className="links__colm-link" href="">Pricing</a>
          <a className="links__colm-link" href="">Changelog</a>
          <a className="links__colm-link" href="">Self-Hosted</a>
          <a className="links__colm-link" href="">Gitpod vs GitHub</a>
          <a className="links__colm-link" href="">Codespaces</a>
          <a className="links__colm-link" href="">Status</a>
        </div>
        <div className="links__colm1">
          <a className="links__colm-link" href=""><span>Developer</span></a>
          <a className="links__colm-link" href="">Getting started</a>
          <a className="links__colm-link" href="">Screencasts</a>
          <a className="links__colm-link" href="">Blog</a>
          <a className="links__colm-link" href="">Documentation</a>
          <a className="links__colm-link" href="">Report a bug</a>
          <a className="links__colm-link" href="">Community</a>
        </div>
        <div className="links__colm1">
          <a className="links__colm-link" href=""><span>Company</span></a>
          <a className="links__colm-link" href="">About</a>
          <a className="links__colm-link" href="">Careers</a>
          <a className="links__colm-link" href="">Contact</a>
          <a className="links__colm-link" href="">Media Kit</a>
        </div>
        <div className="links__colm1">
          <a className="links__colm-link" href=""><span>Legal</span></a>
          <a className="links__colm-link" href="">Imprint</a>
          <a className="links__colm-link" href="">Terms of Service</a>
          <a className="links__colm-link" href="">Privacy Policy</a>
        </div>
      </div>
      <span class="links-line"></span>
      <div class="links__icons">
        <a href="/" className="links__logo">
          <img src="../assets/logo2.svg" alt="logo" />
          <span className="links__text">Copyright © 2021 Gitpod</span>
        </a>
        <div class="icons-link">
          <img src="../assets/twit.svg" alt="twit" />
          <img src="../assets/git2.svg" alt="git" />
          <img src="../assets/mess.svg" alt="mess" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
.links {
  background: #f9f9f9;
  &_container {
    padding: 47px 279px;
    @media only screen and (max-width: 984px) {
      padding: 47px 163px;
    }

    @media only screen and (max-width: 786px) {
      padding: 47px 15px;
    }
  }
  &-colums {
    display: flex;
    justify-content: space-between;
  }

  &__colm1 {
    display: flex;
    flex-direction: column;
    gap: 7px;
  }

  &__colm-link {
    color: $text-color;
    font-size: 13px;
    font-weight: 400;
    line-height: 19.5px;

    transition: 0.4s;

    &:hover{
      color: rgb(255, 183, 0);
      

    }

    @media only screen and (max-width: 425px) {
      font-size: 10px;
    }

    span {
      color: $black;
      font-size: 13px;
      font-weight: 700;
      line-height: 19.5px;
      @media only screen and (max-width: 425px) {
      font-size: 10px;
    }
    }
  }

  &-line {
    display: flex;
    max-width: 852px;
    height: 1px;
    background: #ece7e5;
    margin-top: 47px;
    margin-bottom: 32px;
  }

  &__icons {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  &__logo {
    display: flex;
    gap: 8px;
    align-items: center;
  }

  &__text {
    color: $text-color;
    font-size: 13px;
    font-weight: 400;
    line-height: 19.5px;
  }

  .icons-link {
    display: flex;
    gap: 16px;
    cursor: pointer;
  }
}
</style>
