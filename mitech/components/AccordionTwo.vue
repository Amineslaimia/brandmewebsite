<template>
  <div id="accordion-two">
    <b-card no-body>
      <b-card-header header-tag="header">
        <h5 class="mb-0 font-weight--bold">
          <b-button block v-b-toggle.accordion-one class="btn-link">
            Customizable
            <span>
              <i class="far fa-caret-circle-down"></i>
              <i class="far fa-caret-circle-right"></i>
            </span>
          </b-button>
        </h5>
      </b-card-header>
      <b-collapse id="accordion-one" accordion="my-accordion">
        <b-card-body>
          <b-card-text>
            <div style="color:#2b2b2b">
              it digs dipper into the specificities of each business to help
              create an incomparable and unique value added solving clients'
              real problems and generating steady incomes.
            </div>
          </b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>

    <b-card no-body>
      <b-card-header header-tag="header">
        <h5 class="mb-0 font-weight--bold">
          <b-button block v-b-toggle.accordion-two class="btn-link">
            A strategic approach
            <span>
              <i class="far fa-caret-circle-down"></i>
              <i class="far fa-caret-circle-right"></i>
            </span>
          </b-button>
        </h5>
      </b-card-header>
      <b-collapse id="accordion-two" accordion="my-accordion">
        <b-card-body>
          <b-card-text>
            <div style="color:#2b2b2b">
              it is composed of ten interconnected and easy to follow steps.
            </div>
          </b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>

    <b-card no-body>
      <b-card-header header-tag="header">
        <h5 class="mb-0 font-weight--bold">
          <b-button block v-b-toggle.accordion-three class="btn-link">
            Practical
            <span>
              <i class="far fa-caret-circle-down"></i>
              <i class="far fa-caret-circle-right"></i>
            </span>
          </b-button>
        </h5>
      </b-card-header>
      <b-collapse id="accordion-three" accordion="my-accordion">
        <b-card-body>
          <b-card-text>
            <div style="color:#2b2b2b">
              It provides you with a whole set of simple but not simplistic
              tools & techniques.
            </div>
          </b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>

    <b-card no-body>
      <b-card-header header-tag="header">
        <h5 class="mb-0 font-weight--bold">
          <b-button block v-b-toggle.accordion-four class="btn-link">
            Flexible
            <span>
              <i class="far fa-caret-circle-down"></i>
              <i class="far fa-caret-circle-right"></i>
            </span>
          </b-button>
        </h5>
      </b-card-header>
      <b-collapse id="accordion-four" accordion="my-accordion">
        <b-card-body>
          <b-card-text>
            <div style="color:#2b2b2b">
              you can do it at your own pace depending on your availability by
              purchasing the Do It Yourself (DIY) package. You can just download
              the material follow the tutorials and if need be reach out to the
              technical support to tweak additional things.
            </div>
          </b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>
    <b-card no-body>
      <b-card-header header-tag="header">
        <h5 class="mb-0 font-weight--bold">
          <b-button block v-b-toggle.accordion-five class="btn-link">
            Interactive
            <span>
              <i class="far fa-caret-circle-down"></i>
              <i class="far fa-caret-circle-right"></i>
            </span>
          </b-button>
        </h5>
      </b-card-header>
      <b-collapse id="accordion-five" accordion="my-accordion">
        <b-card-body>
          <b-card-text>
            <div style="color:#2b2b2b">
              an expert will walk you through the whole journey, if your
              purchase the full package version of it, and work hand in hand
              with you until you establish your project and get it to start
              generating incomes.
            </div>
          </b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>
    <b-card no-body>
      <b-card-header header-tag="header">
        <h5 class="mb-0 font-weight--bold">
          <b-button block v-b-toggle.accordion-six class="btn-link">
            Affordable
            <span>
              <i class="far fa-caret-circle-down"></i>
              <i class="far fa-caret-circle-right"></i>
            </span>
          </b-button>
        </h5>
      </b-card-header>
      <b-collapse id="accordion-six" accordion="my-accordion">
        <b-card-body>
          <b-card-text>
            <div style="color:#2b2b2b">
              the price is extremely competitive and comes with extra free
              branding services that are usually expensive if bought apart
              (website creation, social media management, data analysis).
            </div>
          </b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>
  </div>
</template>
