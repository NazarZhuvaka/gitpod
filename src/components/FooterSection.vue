<template>
  <div class="footer">
    <div className="footer_container">
      <h3 class="footer__title">
        This website uses cookies to enhance the user experience. Read our
        <a href="/"> privacy policy </a>
        for more info.
      </h3>
      <button class="footer__btn">Accept Cookies</button>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
.footer {
  &_container {
    padding: 12px 16px;
    display: flex;
    justify-content: space-between;
    background: #ece7e5;
    align-items: center;
  }

  &__title {
    color: $text-color;
    font-size: 16px;
    font-weight: 400;
    line-height: 24px;
    @media only screen and (max-width: 786px) {
      font-size: 11px;
    }

    a{
      text-decoration: underline;
    }
  }
  &__btn {
    border-radius: 8px;
    background: $white;
    border: none;
    padding: 4px 24px;
    color: $text-color;
    text-align: center;
    font-size: 16px;
    font-weight: 400;
    line-height: 24px;

    transition: 0.7s;

    &:hover{
      color:white;
      background: orange;
  }

    @media only screen and (max-width: 786px) {
      font-size: 13px;
    }
    @media only screen and (max-width: 425px) {
      font-size: 11px;
      line-height: 13px;
      padding: 4px 14px;
    }
  }
}
</style>
