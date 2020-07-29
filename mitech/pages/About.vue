<template>
  <div class="main-container">
    <Header />

    <AboutCompanyTwo />

    <TeamTwo class="bg-gray" />

    <Footer />

    <OffCanvasMobileMenu />
  </div>
</template>

<script>
import Header from "@/components/Header";
import TeamTwo from "@/components/sections/TeamTwo";
import PageHeader from "@/components/PageHeader";
import AboutCompanyTwo from "@/components/AboutCompanyTwo";
import CtaFour from "@/components/CtaFour";
import AboutDelivery from "@/components/AboutDelivery";
import FunFactTwo from "@/components/FunFactTwo";
import TestimonialTwo from "@/components/sections/TestimonialTwo";
import BrandLogoCarousel from "@/components/BrandLogoCarousel";
import ContactUsThree from "@/components/sections/ContactUsThree";
import Footer from "@/components/Footer";
import OffCanvasMobileMenu from "@/components/OffCanvasMobileMenu";

export default {
  name: "about",
  components: {
    Header,
    PageHeader,
    TeamTwo,
    AboutCompanyTwo,
    CtaFour,
    AboutDelivery,
    FunFactTwo,
    TestimonialTwo,
    BrandLogoCarousel,
    ContactUsThree,
    Footer,
    OffCanvasMobileMenu
  },
  head() {
    return {
      title: "About Us",
      meta: [
        {
          hid: "description",
          name: "description",
          content: "About our description"
        }
      ]
    };
  }
};
</script>
