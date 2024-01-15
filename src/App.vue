
<template>
  <div class="wrapper">
    <div class="container">
      <HeaderSection/>
      <WelcomeSection/>
      <SelectSection/>
      <CodeSection/>
      <SecureSection/>
      <div class="slider-section" id="app">
        <SliderSection />
      </div>
      <StartSection/>
      <LinksSection/>
      <FooterSection/>

      <!-- <div id="app">
        <SliderSection />
      </div> -->

    </div>
  </div>
</template>

<script>

import SliderSection from './components/SliderSection.vue';


import HeaderSection from './components/HeaderSection.vue'
import WelcomeSection from './components/WelcomeSection.vue'
import SelectSection from './components/SelectSection.vue'
import CodeSection from './components/CodeSection.vue'
import SecureSection from './components/SecureSection.vue'
// import DevSection from './components/DevSection.vue'
import StartSection from './components/StartSection.vue'
import LinksSection from './components/LinksSection.vue'
import FooterSection from './components/FooterSection.vue'



export default {
  name: 'App',
  components: {
    HeaderSection,
    WelcomeSection,
    SelectSection,
    CodeSection,
    SecureSection,
    // DevSection,
    StartSection,
    LinksSection,
    FooterSection,
    SliderSection
        
  }
}
</script>

<style lang="scss">
@import '@/styles/reset.scss';


.wrapper{
  max-width: 1920px;
  margin-inline: auto;

.container{
  max-width: 1408px;
  margin-inline: auto;
  background: $bg-white;
  }

  .slider-section{
    padding: 0px 65px;
  }
}

</style>
