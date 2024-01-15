<template>
  <div class="welcome">
    <div className="welcome_container">
      <div className="welcome__info">
        <h1 className="welcome__info-title">
          Always <br />
          Ready to Code.
        </h1>
        <p className="welcome__info-text">
          Spin up fresh, automated dev environments for each task, in the cloud,
          in seconds.
        </p>
        <div className="welcome__int">
          <button className="welcome__btn">Try Now</button>
          <button className="welcome__btn-sec">
            Open a workspace. <br />
            Start from any Git context.
          </button>
        </div>
        <div class="welcome__icon">
          <img src="../assets/fox.svg" alt="fox" />
          <img src="../assets/git.svg" alt="git" />
          <img src="../assets/blue.svg" alt="blue" />
        </div>
      </div>
      <div className="welcome__img-section">
        <img
          className="welcome__img"
          src="../assets/welcome-img.png"
          alt="img"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
.welcome {
  padding: 0 49px;

  &__img{
    animation: animate 5s ease-in-out infinite;

        @keyframes animate {
            0%,100% 
            {
                transform: translateY(-30px);
            }
            50%
            {
                transform: translateY(40px);
            }
        }
  }
  &_container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 52px;
    margin-bottom: 176px;

    @media only screen and (max-width: 984px) {
      flex-direction: column-reverse;
      gap: 40px;
    }
  }

  &__info-title {
    color: $black;
    font-size: 80px;
    font-weight: 700;
    line-height: 88px;
    margin-bottom: 38px;
    @media only screen and (max-width: 768px) {
      font-size: 69px;
    }

    @media only screen and (max-width: 425px) {
        line-height: 55px;
        font-size: 45px;
    }
  }

  &__info-text {
    color: $text-color;
    font-size: 23px;
    font-weight: 400;
    line-height: 31.92px;
    max-width: 460px;
    margin-bottom: 48px;
    @media only screen and (max-width: 768px) {
      font-size: 21px;
    }
  }

  &__int {
    display: flex;
    gap: 24px;
    margin-bottom: 20px;
  }

  &__btn {
    border-radius: 16px;
    background: $btn-color;
    box-shadow: 0px 1px 1px 0px rgba(0, 0, 0, 0.1);
    padding: 11px 46px;
    border: none;
    color: $black;
    text-align: center;
    font-size: 18px;
    font-weight: 700;
    line-height: 22.5px;
    transition: 0.7s;

    &:hover{
        background: #e3b164;
    }

    @media only screen and (max-width: 425px) {
        font-size: 14px;
    padding: 10px 39px;
    }

    &-sec {
      display: contents;

    }
  }

  &__icon {
    display: flex;
    gap: 28px;
  }
}
</style>
