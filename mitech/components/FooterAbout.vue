<template>
  <div class="footer-widget">
    <div class="footer-widget__logo mb-30">
      <n-link to="/">
        <img
          src="../static/images/logo/brandmelogofooter.png"
          class="img-fluid"
          alt="logo"
        />
      </n-link>
    </div>
    <ul class="footer-widget__list">
      <li>{{ footerAbout.address }}</li>
      <li>
        <a href="mailto:contact@mitech.com" class="hover-style-link">{{
          footerAbout.email
        }}</a>
      </li>
      <li>
        <a
          href="tel:123344556"
          class="hover-style-link text-black font-weight--bold"
        ></a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  props: ["footerAbout"]
};
</script>
