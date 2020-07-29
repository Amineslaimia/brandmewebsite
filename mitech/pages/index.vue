<template>
  <div class="main-container">
    <Header />

    <CtaVideo />

    <HeroInfotechNo />

    <ServiceOne />
    <TeamTwo class="bg-gray" />
    <CtaContact />

    <Footer />

    <OffCanvasMobileMenu />
  </div>
</template>

<script>
import TeamTwo from "@/components/sections/TeamTwo";
import Header from "@/components/Header";
import HeroInfotechNo from "@/components/HeroInfotechNo";
import BrandLogoCarousel from "@/components/BrandLogoCarousel";
import ServiceOne from "@/components/ServiceOne";
import InfoTechExperience from "@/components/sections/InfoTechExperience";
import FunFact from "@/components/FunFact";
import CtaVideo from "@/components/CtaVideo";
import CaseStudiesSection from "@/components/sections/CaseStudiesSection";
import TestimonialOne from "@/components/sections/TestimonialOne";
import BlogStyleOne from "@/components/sections/BlogStyleOne";
import CtaContact from "@/components/CtaContact";
import Footer from "@/components/Footer";
import OffCanvasMobileMenu from "@/components/OffCanvasMobileMenu";

export default {
  components: {
    Header,
    TeamTwo,
    HeroInfotechNo,
    BrandLogoCarousel,
    ServiceOne,
    InfoTechExperience,
    FunFact,
    CtaVideo,
    CaseStudiesSection,
    TestimonialOne,
    BlogStyleOne,
    CtaContact,
    Footer,
    OffCanvasMobileMenu
  },
  head() {
    return {
      title: "Mitech || Infotechnology"
    };
  }
};
</script>
