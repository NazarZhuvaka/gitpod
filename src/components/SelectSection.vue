<template>
  <div class="select">
    <div className="select_container">
      <p class="select__title">Select project,</p>
      <p class="select__text">check dependencies, checkout branch, view</p>
      <p class="select__text">
        readme.txt, install tools, run build, run test,
      </p>
      <p class="select__title">start coding.</p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
.select__title {
  color: $black;
  text-align: center;
  font-size: 54px;
  font-weight: 700;
  line-height: 63.72px;

  @media only screen and (max-width: 984px) {
    font-size: 46px;
  }

  @media only screen and (max-width: 768px) {
    font-size: 34px;
  }

  @media only screen and (max-width: 425px) {
    font-size: 25px;
    line-height: 37.72px;
  }
}
.select__text {
  color: $gray;
  text-align: center;
  font-size: 54px;
  font-weight: 400;
  line-height: 63.72px;
  text-decoration-line: line-through;

  @media only screen and (max-width: 984px) {
    font-size: 46px;
  }

  @media only screen and (max-width: 768px) {
    font-size: 34px;
  }

  @media only screen and (max-width: 425px) {
    line-height: 37.72px;
    font-size: 21px;
  }
}
</style>
