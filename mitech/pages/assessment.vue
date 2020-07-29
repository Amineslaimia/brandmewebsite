<template>
  <div class="main-container">
    <Header />

    <Breadcrumbs
      breadcrumbTitle="Assess Your Readiness

"
    />
    <div class="col-lg-5 offset-lg-5">
      <div>title</div>
      <div style="font-family: 'ObjectiveLight'; font-size:10px">
        Rate yourself from 0 to 10 on the following sentences
      </div>
    </div>
    <form>
      <div class="page" v-for="k in page1.USPReadiness" :key="k">
        <div class="col-lg-5 offset-lg-4 ">
          <div class="text">
            {{ k.question }}

            <div id="debt-amount-slider" v-for="item in k.choices" :key="item">
              <div class="container">
                <label :for="item.value">{{ item.choice }} </label>
                <input
                  type="radio"
                  :name="k.id"
                  :id="item.value"
                  :value="item.value"
                />
              </div>
            </div>
          </div>
        </div>
      </div>
    </form>
    <button type="submit">Get Debt Free!</button>

    <Footer />

    <OffCanvasMobileMenu />
  </div>
</template>

<script>
import Header from "@/components/Header";
import survey from "@/components/survey";
import Breadcrumbs from "@/components/Breadcrumbs";
import ContactUsFour from "@/components/sections/ContactUsFour";
import CtaOne from "@/components/CtaOne";
import Footer from "@/components/Footer";
import page1 from "../data/page1.json";
import page2 from "../data/page2.json";
import page3 from "../data/page3.json";
import page4 from "../data/page4.json";
import page5 from "../data/page5.json";
import page6 from "../data/page6.json";
import page7 from "../data/page7.json";
import page8 from "../data/page8.json";

import OffCanvasMobileMenu from "@/components/OffCanvasMobileMenu";

export default {
  name: "contact",
  components: {
    Header,
    survey,
    Breadcrumbs,
    ContactUsFour,
    CtaOne,
    Footer,
    OffCanvasMobileMenu
  },
  head() {
    return {
      title: "Contact Us"
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
          text: "Contact Us",
          active: true
        }
      ],

      page1,
      page2,
      page3,
      page4,
      page5,
      page6,
      page7,
      page8
    };
  }
};
</script>
