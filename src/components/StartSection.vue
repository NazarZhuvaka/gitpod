<template>
  <div class="start">
    <div className="start_container">
      <h3 class="start__title">Get started now</h3>
      <div class="start-cards">
        <div class="start__connect">
          <h4 class="start__connect__title">Connect Git repository</h4>
          <p class="start__connect__welcome">
            Select a Git provider to start with an existing project from any Git
            context.
          </p>
          <div class="start__connect__with">
            <div class="start__connect__btn">
              <img src="../assets/fox.svg" alt="fox" />
              Continue with GitLab
            </div>
            <div class="start__connect__btn" id="black">
              <img src="../assets/git3.svg" alt="git" />
              Continue with GitHub
            </div>
            <div class="start__connect__btn" id="blue">
              <img src="../assets/blue3.svg" alt="blue" />
              Continue with Bitbucket
            </div>
          </div>
          <p class="start__text">
            Or prefix any GitLab, GitHub or Bitbucket URL with
          </p>
          <a class="start__link" href="/"> gitpod.io/# </a>
        </div>
        <div class="start__launch">
          <h4 class="start__connect__title">Launch an example workspace</h4>
          <p class="start__connect__welcome" id="welcome">
            Dive into one of our example workspaces
          </p>
          <div class="start__launch__with">
            <div class="start__launch__btn">
              <div class="start__launch__icon">
                <img src="../assets/getstart/ts.svg" alt="TypeScript" />
                Node or TypeScript
              </div>
              <button class="start-btn">Launch workspace</button>
            </div>
            <div class="start__launch__btn">
              <div class="start__launch__icon">
                <img src="../assets/getstart/py.svg" alt="python" />
                Python
              </div>
              <button class="start-btn">Launch workspace</button>
            </div>
            <div class="start__launch__btn">
              <div class="start__launch__icon">
                <img src="../assets/getstart/go.svg" alt="Go" />
                Go
              </div>
              <button class="start-btn">Launch workspace</button>
            </div>

            <div class="start__launch__btn">
              <div class="start__launch__icon">
                <img src="../assets/getstart/rust.svg" alt="Rust" />
                Rust
              </div>
              <button class="start-btn">Launch workspace</button>
            </div>
            <div class="start__launch__btn">
              <div class="start__launch__icon">
                <img src="../assets/getstart/java.svg" alt="Java" />
                Java
              </div>
              <button class="start-btn">Launch workspace</button>
            </div>
            <div class="start__launch__btn">
              <div class="start__launch__icon">
                <img src="../assets/getstart/sv.svg" alt="Svelte" />
                Svelte
              </div>
              <button class="start-btn">Launch workspace</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
.start {
  &-cards {
    padding: 0 20px;

    @media only screen and (max-width: 1300px) {
      flex-direction: column;
      align-items: center;
    }
  }

  &_container {
    margin-bottom: 160px;
  }
  &__title {
    color: $black;
    text-align: center;
    font-size: 54px;
    font-weight: 700;
    line-height: 71.82px;
    margin-top: 177px;
    margin-bottom: 48px;

    @media only screen and (max-width: 768px) {
      margin-top: 120px;

      font-size: 46px;
    }

    @media only screen and (max-width: 425px) {
      font-size: 35px;
    }
  }

  &__text {
    color: rgba(18, 16, 12, 0.7);
    text-align: center;
    font-size: 24px;
    font-weight: 400;
    line-height: 31.92px;
    max-width: 486px;
    margin-bottom: 6px;

    @media only screen and (max-width: 425px) {
      font-size: 18px;
    }
  }

  &__link {
    color: rgba(18, 16, 12, 0.7);
    text-align: center;
    font-size: 24px;
    font-weight: 400;
    line-height: 31.92px;
    border-radius: 12px;
    background: #ffe4bc;
    padding: 1px 16px;
    display: flex;
    max-width: 151px;
    margin-inline: auto;

    @media only screen and (max-width: 425px) {
      font-size: 18px;
    }
  }

  &-cards {
    display: flex;
    gap: 26px;
    justify-content: center;
  }

  &__connect {
    border-radius: 20px;
    background: #fff;
    padding: 56px 78px 86px;
    max-width: 643px;

    &__with {
      display: flex;
      flex-direction: column;
      gap: 16px;
      justify-content: center;
      align-items: center;
      margin-bottom: 64px;
    }

    &__title {
      color: $black;
      text-align: center;
      font-size: 32px;
      font-weight: 700;
      line-height: 40px;
      margin-bottom: 8px;

      @media only screen and (max-width: 425px) {
        font-size: 28px;
        line-height: 33px;
      }
    }

    &__welcome {
      color: $text-color;
      text-align: center;
      font-size: 24px;
      font-weight: 400;
      line-height: 31.92px;
      max-width: 471px;
      margin-bottom: 62px;
      margin-inline: auto;

      @media only screen and (max-width: 425px) {
        font-size: 20px;
      }
    }

    #black {
      background: #000;
    }
    #blue {
      background: #2684ff;
    }

    &__btn {
      border-radius: 12px;
      background: $btn-color-org;
      box-shadow: 0px 1px 1px 0px rgba(0, 0, 0, 0.1);
      display: flex;
      align-items: center;
      padding: 9px 33px;
      gap: 16px;
      max-width: 262px;
      color: #fff;
      text-align: center;
      font-size: 14px;
      font-weight: 700;
      line-height: 16px;
      width: 100%;
    }
  }

  #welcome {
    margin-bottom: 20px;
    font-size: 23px;
  }

  &__launch {
    border-radius: 20px;
    background: #fff;
    padding: 56px 56px 86px;
    max-width: 642px;
    width: 100%;

    &__icon {
      display: flex;
      align-items: center;
      gap: 16px;

      color: $text-color;
      text-align: center;
      font-size: 20px;
      font-weight: 400;
      line-height: 20px;

      @media only screen and (max-width: 425px) {
        font-size: 12px;
        gap: 4px;
      }
    }

    &__btn {
      border-radius: 12px;
      background: #f9f9f9;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 12px;
      margin-top: 12px;
      max-width: 530px;
    }
  }
  &-btn {
    border-radius: 12px;
    background: $black;
    box-shadow: 0px 1px 1px 0px rgba(0, 0, 0, 0.1);
    color: #fff;
    text-align: center;
    font-size: 14px;
    font-weight: 400;
    line-height: 16px;
    padding: 8px 12px;
    border: none;

    transition: 0.6s;

    &:hover{
      color:black;
      background: white;
  }

    @media only screen and (max-width: 425px) {
      font-size: 9px;
      padding: 6px 5px;
    }
  }
}
</style>
