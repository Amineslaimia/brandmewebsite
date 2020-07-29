<template>
  <div class="main-container">
    <Header />

    <div
      class="about-banner-wrap banner-space bg-cover"
      style="background-image: url('images/bg/animateme.png');padding-top: 360px;padding-bottom: 200px;"
    ></div>

    <Footer />

    <OffCanvasMobileMenu />
  </div>
</template>

<script>
import Header from "@/components/Header";
import Breadcrumbs from "@/components/Breadcrumbs";
import ServiceIT from "@/components/ServiceIT";
import ContactUsThree from "@/components/sections/ContactUsThree";
import Footer from "@/components/Footer";
import OffCanvasMobileMenu from "@/components/OffCanvasMobileMenu";

export default {
  components: {
    Header,
    Breadcrumbs,
    ServiceIT,
    ContactUsThree,
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
