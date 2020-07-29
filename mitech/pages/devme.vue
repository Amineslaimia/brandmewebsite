<template>
  <div class="main-container">
    <Header />

    <div
      class="about-banner-wrap banner-space bg-cover"
      style="background-image: url('images/bg/devme.png');padding-top: 360px;padding-bottom: 200px;"
    ></div>
    <div class="feature-large-images-wrapper section-space--ptb_100 pb-md-sm-0">
      <div class="container">
        <div class="cybersecurity-about-box">
          <div class="row">
            <div class="col-lg-6">
              <div class="modern-number-01">
                <h5 class="heading mt-0">
                  Your products or services go unnoticed in your

                  <span class="text-color-primary"> current website?</span>
                </h5>
              </div>
            </div>
            <div class="col-lg-5 offset-lg-1">
              <div class="conact-us-wrap-one managed-it">
                <h6 class="heading">
                  DevMe is more than a place for web development. It is a place
                  for you to craft powerful visual attractive marketing messages
                  to highlight your
                  <span class="text-color-primary">
                    Unique Selling Proposition and win clients.</span
                  >
                </h6>

                <div class="sub-heading"></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="feature-icon-wrapper section-space--pb_70">
      <div class="container">
        <div class="row">
          <div class="col-lg-12">
            <div class="section-title-wrap text-center section-space--mb_20">
              <h3 class="heading">DevMe services</h3>
            </div>
          </div>
        </div>
        <div class="row">
          <div class="col-12">
            <div class="feature-list__three">
              <div class="row">
                <div class="col-lg-6">
                  <div class="grid-item animate">
                    <div class="ht-box-icon style-03">
                      <div class="icon-box-wrap">
                        <div class="content-header">
                          <div class="icon">
                            <i class="	fa fa-balance-scale"></i>
                          </div>
                          <h5 class="heading">
                            Websites that are:
                          </h5>
                        </div>
                        <div class="content">
                          <div class="text">
                            <ul>
                              <li>User-friendly</li>

                              <li>Professional</li>
                              <li>Affordabley</li>
                            </ul>
                          </div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="col-lg-6">
                  <div class="grid-item animate">
                    <div class="ht-box-icon style-03">
                      <div class="icon-box-wrap">
                        <div class="content-header">
                          <div class="icon">
                            <i class="fa fa-book"></i>
                          </div>
                          <h5 class="heading">
                            SEO set-up
                          </h5>
                        </div>
                        <div class="content">
                          <div class="text"></div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="col-lg-6">
                  <div class="grid-item animate">
                    <div class="ht-box-icon style-03">
                      <div class="icon-box-wrap">
                        <div class="content-header">
                          <div class="icon">
                            <i class="	fa fa-edit"></i>
                          </div>
                          <h5 class="heading">
                            Email connection
                          </h5>
                        </div>
                        <div class="content">
                          <div class="text"></div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="col-lg-6">
                  <div class="grid-item animate">
                    <div class="ht-box-icon style-03">
                      <div class="icon-box-wrap">
                        <div class="content-header">
                          <div class="icon">
                            <i class="fa fa-handshake"></i>
                          </div>
                          <h5 class="heading">
                            Mobile apps development
                          </h5>
                        </div>
                        <div class="content">
                          <div class="text"></div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="col-lg-6">
                  <div class="grid-item animate">
                    <div class="ht-box-icon style-03">
                      <div class="icon-box-wrap">
                        <div class="content-header">
                          <div class="icon">
                            <i class="fa fa-users"></i>
                          </div>
                          <h5 class="heading">
                            Support & maintenance
                          </h5>
                        </div>
                        <div class="content">
                          <div class="text"></div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <CtaThree />
    <Footer />

    <OffCanvasMobileMenu />
  </div>
</template>

<script>
import Header from "@/components/Header";
import Breadcrumbs from "@/components/Breadcrumbs";
import ServiceIT from "@/components/ServiceIT";
import CtaThree from "@/components/CtaThree";
import Footer from "@/components/Footer";
import OffCanvasMobileMenu from "@/components/OffCanvasMobileMenu";

export default {
  components: {
    Header,
    Breadcrumbs,
    CtaThree,
    ServiceIT,

    Footer,
    OffCanvasMobileMenu
  },
  head() {
    return {
      title: "IT Services"
    };
  },
  data() {
    return {
      breadcrumbNavigation: [
        {
          text: "Home",
          to: "/"
        },
        {
          text: "IT-Services",
          active: true
        }
      ]
    };
  }
};
</script>
