<script>
import HeaderSection from '../components/HeaderSection.vue';
import ServiceSection from '../components/ServiceSection.vue';
import CompanyValuesSection from '../components/CompanyValuesSection.vue';
import AboutUsSection from '../components/AboutUsSection.vue';
import ContactInfoSection from '../components/ContactInfoSection.vue';
import FooterComponent from '../components/FooterComponent.vue';
import NavbarComponent from '../components/NavbarComponent.vue';

export default {
  components: {
    HeaderSection,
    ServiceSection,
    CompanyValuesSection,
    AboutUsSection,
    ContactInfoSection,
    FooterComponent,
    NavbarComponent,
  },
};
</script>

<template>
  <div>
    <navbar>
      <NavbarComponent class="navbar" />
    </navbar>
    <section id="header">
      <HeaderSection class="container" />
    </section>
    <section id="service">
      <ServiceSection class="container" />
    </section>
    <section id="company">
      <CompanyValuesSection class="container" />
    </section>
    <section id="about">
      <AboutUsSection class="container" />
    </section>
    <section id="contact">
      <ContactInfoSection class="container" />
    </section>
    <footer>
      <FooterComponent class="footer" />
    </footer>
  </div>
</template>

<style scoped>
section {
  height: 100vh;
  width: 100%;
  background-color: white;
}

footer {
  width: 100%;
  box-shadow: -3px -1px 2px rgba(0, 0, 0, 0.4);
}
navbar {
  width: 100%;
  box-shadow: -3px 0px 2px rgba(0, 0, 0, 0.4);
  background-color: white;
  position: fixed;
}

.navbar {
  margin: auto;
  padding: 12px 0px;
  width: 90%;
}
.container {
  margin: auto;
  width: 90%;
  padding: 72px 0px;
}
.footer {
  margin: auto;
  padding: 12px 0px;
  width: 90%;
}
</style>
