<template>
  <div class="feature-large-images-wrapper section-space--ptb_100">
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div class="section-title-wrap text-center section-space--mb_60">
            <h6 class="section-sub-title mb-20">
              {{ data.aboutCompanyTwo.sectionSubTitle }}
            </h6>
            <h3 class="heading" v-html="data.aboutCompanyTwo.sectionTitle">
              {{ data.aboutCompanyTwo.sectionTitle }}
            </h3>
          </div>
        </div>
      </div>

      <div class="cybersecurity-about-box section-space--pb_70">
        <div class="row" style="margin-bottom:3vh">
          <div class="col-lg-4 offset-lg-1">
            <div class="modern-number-01">
              <h2 class="heading mr-5">
                <span class="mark-text" style="opacity:10%">{{
                  data.aboutCompanyTwo.headingMarkText
                }}</span>
              </h2>
            </div>
          </div>

          <div class="col-lg-5 offset-lg-1">
            <div class="cybersecurity-about-text">
              <div class="text" style="font-family: 'ObjectiveMedium';font-size:21px">
                {{ data.aboutCompanyTwo.desc }}
              </div>
              <div class="button-text">
                <n-link to="/brandwiser" class="btn-text">
                  learn more about BRANDWISER
                  <span class="button-icon ml-1">
                    <i class="far fa-long-arrow-right"></i>
                  </span>
                </n-link>
              </div>
            </div>
          </div>
        </div>
        <div class="row" style="margin-bottom:3vh">
          <div class="col-lg-4 offset-lg-1">
            <div class="modern-number-01">
              <h2 class="heading mr-5">
                <span class="mark-text" style="opacity:10%">Vision</span>
              </h2>
            </div>
          </div>

          <div class="col-lg-5 offset-lg-1">
            <div class="cybersecurity-about-text">
              <div class="text" style="font-family: 'ObjectiveMedium';font-size:30px">
                To create brands that last
              </div>
              <div class="button-text"></div>
            </div>
          </div>
        </div>
        <div class="row" >
          <div class="col-lg-4 offset-lg-1">
            <div class="modern-number-01">
              <h2 class="heading mr-5">
                <span class="mark-text" style="opacity:10%">Values</span>
              </h2>
            </div>
          </div>

          <div class="col-lg-5 offset-lg-1">
            <div class="cybersecurity-about-text">
              <div
                class="text"
                style="font-family: 'ObjectiveMedium'; font-size:30px"
              >
                Creativity, </br> Innovation,</br> No mass branduction
              </div>
              <div class="button-text"></div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import data from "../data/about.json";
export default {
  data() {
    return {
      data
    };
  }
};
</script>
