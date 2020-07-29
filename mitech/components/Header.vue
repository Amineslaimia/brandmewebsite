<template>
  <div class="header-area header-area--default">
    <fixed-header :threshold="10">
      <div class="header-bottom-wrap">
        <div class="container-fluid">
          <div class="row">
            <div class="col-lg-12">
              <div class="header default-menu-style position-relative">
                <a id="logolink">
                  <div class="header__logo">
                    <n-link to="/">
                      <img
                        id="secondb"
                        src="images/logo/secondbb.png"
                        class="secondb"
                        alt="Brand Logo"
                      />

                      <img
                        id="firstb"
                        src="images/logo/firstbb.png"
                        class="firstb"
                        alt="Brand Logo"
                      />

                      <img
                        id="randme"
                        src="images/logo/randme.png"
                        class="randme"
                        alt="Brand Logo"
                      />
                    </n-link>
                  </div>
                </a>
                <div class="header-midle-box">
                  <div class="header-bottom-wrap d-md-block d-none">
                    <div class="header-bottom-inner">
                      <div class="header-bottom-left-wrap">
                        <div class="header__navigation d-none d-xl-block">
                          <nav class="navigation-menu primary--menu">
                            <Navigation />
                          </nav>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>

                <!-- header right box -->
                <div class="header-right-box">
                  <div class="header-bottom-wrap d-md-block d-none">
                    <div class="header-bottom-inner">
                      <div class="header-bottom-left-wrap">
                        <div class="header__navigation d-none d-xl-block">
                          <nav class="navigation-menu primary--menu">
                            <ul>
                              <li>
                                <n-link to="/about">
                                  <span>About Us</span>
                                </n-link>
                              </li>
                              <li>
                                <n-link to="/contact">
                                  <span>Contact Us</span>
                                </n-link>
                              </li>
                            </ul>
                          </nav>
                        </div>
                      </div>
                    </div>
                  </div>

                  <!-- mobile menu -->
                  <div
                    class="mobile-navigation-icon d-block d-xl-none"
                    id="mobile-menu-trigger"
                    @click="mobiletoggleClass('addClass', 'active')"
                  >
                    <i></i>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </fixed-header>
  </div>
</template>

<script>
import FixedHeader from "vue-fixed-header";
import HeaderTop from "@/components/HeaderTop";
import Navigation from "@/components/Navigation";

export default {
  components: {
    HeaderTop,
    Navigation,
    FixedHeader
  },
  data() {
    return {
      hover: false
    };
  },
  methods: {
    // offcanvas mobilemenu open
    mobiletoggleClass(addRemoveClass, className) {
      const el = document.querySelector("#offcanvas-menu");
      if (addRemoveClass === "addClass") {
        el.classList.add(className);
      } else {
        el.classList.remove(className);
      }
    }
  }
};
</script>
