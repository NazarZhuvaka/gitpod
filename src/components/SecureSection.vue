<template>
  <div class="secure">
    <div className="secure_container">
      <h2 class="secure__title">Remote-first. Secure by design.</h2>
      <div class="secure__img">
        <img src="../assets/secure.png" alt="secure-img" />
      </div>
      <p class="secure__text">
        You no longer need an over-powered laptop to code, Gitpod works just as
        smoothly on a Chromebook or iPad. All you need is a browser. Gitpod
        centralizes all source code and never stores it on insecure machines and
        networks.
      </p>
      <div className="secure__text__int">
        <button className="secure__text__btn">
          <img src="../assets/chrome.svg" alt="chrome" />
          Chrome Extension
        </button>
        <button className="secure__text__btn">
          <img src="../assets/fire-fox.svg" alt="fire-fox" />
          Firefox Extension
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
.secure_container {
  padding: 0px 20px;
}
.secure__title {
  color: $black;
  text-align: center;
  font-size: 54px;
  font-weight: 700;
  line-height: 71.82px;
  margin-top: 337px;

  @media only screen and (max-width: 1300px) {
    margin-top: 237px;
  }

  @media only screen and (max-width: 768px) {
    margin-top: 140px;
    font-size: 46px;
  }

  @media only screen and (max-width: 425px) {
    margin-top: 101px;
    font-size: 30px;
    line-height: 36.82px;
    }
}

.secure__img {
  display: flex;
  justify-content: center;
  margin-top: 30px;
  margin-bottom: 40px;
}

.secure__text {
  color: $text-color;
  text-align: center;
  font-size: 24px;
  font-weight: 400;
  line-height: 31.92px;
  max-width: 875px;
  margin-inline: auto;
  margin-bottom: 45px;

  @media only screen and (max-width: 425px) {
    font-size: 16px;
    }

  &__int {
    display: flex;
    gap: 16px;
    justify-content: center;
  }

  &__btn {
    padding: 7px 12px;
    display: flex;
    gap: 10px;
    align-items: center;

    color: $black;
    text-align: center;
    font-size: 18px;
    font-weight: 700;
    line-height: 31.86px;

    border-radius: 9px;
    background: #fff;
    box-shadow: 0px 0.5px 2px 0px rgba(0, 0, 0, 0.1);
    border: none;

    transition: 0.7s;

    &:hover{
      background: #0f0f0f;
      color: white;
    }

    @media only screen and (max-width: 425px) {
      font-size: 13px;
    line-height: 12.86px;
    }
  }
}
</style>
