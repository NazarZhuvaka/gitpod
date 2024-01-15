<template>
  <div class="code">
    <div className="code_container">
      <div className="code__info">
        <h1 className="code__info-title">Think CI/CD for dev environments</h1>
        <p className="code__info-text">
          We invented prebuilds so application code, configuration and
          infrastructure can all be stored as machine-executable code in your
          git repositories and applied to dev environments automatically and
          continuously.
        </p>
        <div className="code__int">
          <button className="code__btn">More on prebuilds</button>
          <button className="code__btn-sec">Documentation</button>
        </div>
      </div>
      <div className="code__img-container">
        <img className="code__img" src="../assets/code.png" alt="img" />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
.code {
  margin-top: 339px;
  @media only screen and (max-width: 1300px) {
    margin-top: 225px;
  }

  &_container {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0 48px;

    @media only screen and (max-width: 1300px) {
      flex-direction: column-reverse;
      gap: 40px;
      text-align: center;
    }
  }

  &__info-title {
    color: $black;
    font-size: 32px;
    font-weight: 700;
    line-height: 40px;
    margin-bottom: 8px;

    @media only screen and (max-width: 425px) {
      font-size: 28px;
    }
  }

  &__info-text {
    color: $text-color;
    font-size: 24px;
    font-weight: 400;
    line-height: 31.92px;
    max-width: 648px;
    margin-bottom: 151px;
    @media only screen and (max-width: 1300px) {
      margin-bottom: 100px;
    }

    @media only screen and (max-width: 425px) {
      line-height: 30.92px;
      font-size: 16px;
      margin-bottom: 50px;
    }
  }

  &__int {
    display: flex;
    gap: 16px;

    @media only screen and (max-width: 1300px) {
      justify-content: center;
    }
  }

  &__btn {
    border-radius: 16px;
    background: $btn-color;
    box-shadow: 0px 1px 1px 0px rgba(0, 0, 0, 0.1);
    padding: 8px 18px;
    border: none;
    color: $black;
    text-align: center;
    font-size: 14px;
    font-weight: 700;
    line-height: 16px;
    transition: 0.6s;

    &:hover{
        background: #e3b164;
    }

    &-sec {
      border-radius: 10.5px;
      background: $btn-color-sec;
      box-shadow: 0px 1px 1px 0px rgba(0, 0, 0, 0.1);

      color: $black;
      text-align: center;
      font-size: 14px;
      font-weight: 700;
      line-height: 16px;
      padding: 8px 24px;
      border: none;

      transition: 0.6s;

    &:hover{
      background: #c68786;
    }
    }
  }
}
</style>
