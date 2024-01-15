<template>
  <div class="dev">
    <div className="dev_container">
      <h2 class="dev__title">Used by 400,000+ developers.</h2>
    </div>
  </div>

  <Swiper :options="swiperOptions">
    
    <SwiperSlide class="slide-card">
      <p class="slide__title">GitPod is incredibly cool.</p>
      <p class="slide__text">
        In my opinion, this is a big step in open source software contribution.
        I'm excited to see where we go from here.
      </p>
      <div class="slide__worker">
        <img src="../assets/ben.svg" alt="Ben Halpern" />
        <div class="slide__man">
          <h3 class="slide__man__name">Ben Halpern</h3>
          <p class="slide__man__work">
            Creator and Co-founder <span>@forem</span> and
          </p>
          <p class="slide__man__link">@ThePracticalDev</p>
        </div>
      </div>
    </SwiperSlide>
    <SwiperSlide class="slide-card">
      <p class="slide__title">
        Let's say we were overwhelmed how smooth @gitpod workspaces creation &
        own Docker image for workspaces worked.
      </p>
      <p class="slide__text">
        Plus, installing @code extensions from the store and integrating @gitlab
        CI. That blew my mind entirely, and that is hard ;)
      </p>
      <div class="slide__worker">
        <img src="../assets/slider/mich2.svg" alt="mich" />
        <div class="slide__man">
          <h3 class="slide__man__name">Michael Friedrich</h3>
          <p class="slide__man__work">
            Developer Evangelist <span>@GitLab</span>
          </p>
          
        </div>
      </div>
    </SwiperSlide>
    <SwiperSlide class="slide-card">
      <p class="slide__title">GitPod is incredibly cool.</p>
      <p class="slide__text">
        In my opinion, this is a big step in open source software contribution.
        I'm excited to see where we go from here.
      </p>
      <div class="slide__worker">
        <img src="../assets/slider/ju2.svg" alt="ju" />
        <div class="slide__man">
          <h3 class="slide__man__name">Ben Halpern</h3>
          <p class="slide__man__work">
            Creator and Co-founder <span>@forem</span> and
          </p>
          <p class="slide__man__link">@ThePracticalDev</p>
        </div>
      </div>
    </SwiperSlide>
    <SwiperSlide class="slide-card">
      <p class="slide__title">GitPod is incredibly cool.</p>
      <p class="slide__text">
        In my opinion, this is a big step in open source software contribution.
        I'm excited to see where we go from here.
      </p>
      <div class="slide__worker">
        <img src="../assets/slider/david2.svg" alt="Ben Halpern" />
        <div class="slide__man">
          <h3 class="slide__man__name">Ben Halpern</h3>
          <p class="slide__man__work">
            Creator and Co-founder <span>@forem</span> and
          </p>
          <p class="slide__man__link">@ThePracticalDev</p>
        </div>
      </div>
    </SwiperSlide>
    <SwiperSlide class="slide-card">
      <p class="slide__title">GitPod is incredibly cool.</p>
      <p class="slide__text">
        In my opinion, this is a big step in open source software contribution.
        I'm excited to see where we go from here.
      </p>
      <div class="slide__worker">
        <img src="../assets/slider/bart2.svg" alt="Ben Halpern" />
        <div class="slide__man">
          <h3 class="slide__man__name">Ben Halpern</h3>
          <p class="slide__man__work">
            Creator and Co-founder <span>@forem</span> and
          </p>
          <p class="slide__man__link">@ThePracticalDev</p>
        </div>
      </div>
    </SwiperSlide>
  </Swiper>
  <div class="slider__img">
    <img class="slider__img_link" src="../assets/slider/gitlab.svg" alt="" />
    <img class="slider__img_link" src="../assets/slider/freecode.svg" alt="" />
    <img class="slider__img_link" src="../assets/slider/wave.svg" alt="" />
    <img class="slider__img_link" src="../assets/slider/google.svg" alt="" />
    <img class="slider__img_link" src="../assets/slider/amazon.svg" alt="" />
    <img
      class="slider__img_link"
      src="../assets/slider/facebookicon.svg"
      alt=""
    />
    <img class="slider__img_link" src="../assets/slider/uber.svg" alt="" />
    <img class="slider__img_link" src="../assets/slider/ai.svg" alt="" />
    <img class="slider__img_link" src="../assets/slider/intel.svg" alt="" />
    <img class="slider__img_link" src="../assets/slider/theai.svg" alt="" />
    <img class="slider__img_link" src="../assets/slider/code.svg" alt="" />
    <img class="slider__img_link" src="../assets/slider/geeks.svg" alt="" />
  </div>
</template>

<script>
import { Swiper, SwiperSlide } from "swiper/vue";
import "swiper/css";
import "swiper/css/navigation";

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  data() {
    return {
      swiperOptions: {
        slidesPerView: 1,
        spaceBetween: 10,
        navigation: true,
      },
    };
  },
};
</script>

<style scoped lang="scss">
.slider__img {
  display: flex;
  flex-wrap: wrap;
  gap: 67px;
  text-align: center;
  justify-content: center;
  margin-top: 100px;

  @media only screen and (max-width: 984px) {
    gap: 47px;
  }

  @media only screen and (max-width: 425px) {
    margin-top: 60px;
  }

  &_link {
    cursor: pointer;
  }
}
.slide {
  &-card {
    border-radius: 16px;
    background: #fff;
    padding: 24px 31px 24px 24px;
    max-width: 384px;
    margin-right: 20px;
  }

  &__title {
    color: #12100c;
    font-size: 16px;
    font-weight: 400;
    line-height: 24px;
    margin-bottom: 10px;
    @media only screen and (max-width: 425px) {
      font-size: 14px;
  }
  }

  &__text {
    color: #12100c;
    font-size: 16px;
    font-weight: 400;
    line-height: 24px;
    max-width: 329px;
    margin-bottom: 14px;

    @media only screen and (max-width: 425px) {
      font-size: 12px;
  }
  }

  &__worker {
    display: flex;
    gap: 12px;
    
    @media only screen and (max-width: 425px) {
      flex-direction: column;
      max-width: 50%;
  }
  }

  &__man__name {
    color: #12100c;
    font-size: 16px;
    font-weight: 700;
    line-height: 24px;
    margin-bottom: 8px;
    @media only screen and (max-width: 425px) {
      font-size: 12px;
  }
  }

  &__man__work {
    color: #12100c;
    font-size: 16px;
    font-weight: 400;
    line-height: 24px;
    @media only screen and (max-width: 425px) {
      font-size: 11px;
  }
  }

  &__man__link {
    color: #12100c;
    font-size: 16px;
    font-weight: 400;
    line-height: 24px;
    @media only screen and (max-width: 425px) {
      font-size: 11px;
  }
  }

  span {
    color: #12100c;
    font-size: 16px;
    font-weight: 700;
    line-height: 24px;
  }
}

.dev__title {
  color: #12100c;
  text-align: center;
  font-size: 54px;
  font-weight: 700;
  line-height: 63.72px;
  margin-top: 176px;
  margin-bottom: 49px;

  @media only screen and (max-width: 768px) {
    font-size: 46px;
  }

  @media only screen and (max-width: 425px) {
    font-size: 33px;
    margin-top: 104px;
    line-height: 41.72px;
  }
}
</style>
