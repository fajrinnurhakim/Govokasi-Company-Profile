<script>
import HomeSection from '../components/HomeSection.vue';
import ServiceSection from '../components/ServiceSection.vue';
import CompanyValuesSection from '../components/CompanyValuesSection.vue';
import AboutUsSection from '../components/AboutUsSection.vue';
import ContactComponent from '../components/ContactComponent.vue';
import FooterComponent from '../components/FooterComponent.vue';
import HeaderComponent from '../components/HeaderComponent.vue';

export default {
  components: {
    HomeSection,
    ServiceSection,
    CompanyValuesSection,
    AboutUsSection,
    ContactComponent,
    FooterComponent,
    HeaderComponent,
  },
};
</script>

<template>
  <div>
    <navbar>
      <HeaderComponent class="navbar" />
    </navbar>
    <section id="home">
      <HomeSection class="container" />
    </section>
    <section id="about">
      <AboutUsSection class="container" />
    </section>
    <section id="service">
      <ServiceSection class="container" />
    </section>
    <section id="company">
      <CompanyValuesSection class="container" />
    </section>
    <section id="contact">
      <ContactComponent class="container" />
    </section>
    <footer>
      <FooterComponent class="footer" />
    </footer>
  </div>
</template>

<style scoped>
section#home {
  height: 100vh;
  width: 100%;
  background-color: white;
}
section#about {
  height: 100vh;
  width: 100%;
  background-color: white;
}
section#service {
  height: 100vh;
  width: 100%;
  background-color: white;
}
section#company {
  height: 100vh;
  width: 100%;
  background-color: white;
}
section#contact {
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
