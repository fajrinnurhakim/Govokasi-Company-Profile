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
  data() {
    return {
      isSticky: false,
    };
  },
  mounted() {
    this.handleInitialScroll();
    window.addEventListener('scroll', this.handleScroll);
  },
  destroyed() {
    window.removeEventListener('scroll', this.handleScroll);
  },
  methods: {
    handleInitialScroll() {
      if (window.scrollY === 0) {
        this.isSticky = false;
      } else {
        this.isSticky = true;
      }
    },
    handleScroll() {
      if (window.scrollY > 1 && !this.isSticky) {
        this.isSticky = true;
      } else if (window.scrollY === 0 && this.isSticky) {
        this.isSticky = false;
      }
    },
  },
};
</script>

<template>
  <div class="app">
    <navbar class="nav" :class="{ 'sticky-header': isSticky }">
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
      <div class="footer">
        <FooterComponent class="container" />
      </div>
    </footer>
  </div>
</template>

<style scoped>
.app {
  background: linear-gradient(to right, #110f5e, #010021);
}
section#home {
  height: auto;
  width: 100%;
  background: linear-gradient(to right, #110f5e, #010021);
}
section#about {
  height: auto;
  width: 100%;
  background-color: white;
  padding: 36px 0px;
}
section#service {
  height: auto;
  width: 100%;
  background-color: #110f5e;
  padding: 36px 0px;
}
section#company {
  height: auto;
  width: 100%;
  background-color: white;
  padding: 36px 0px;
}
section#contact {
  height: auto;
  width: 100%;
  background-color: #110f5e;
  padding: 36px 0px;
}

footer {
  width: 100%;
  background-color: #ffffff;
}
.footer {
  width: 90%;
  margin: auto;
}
navbar {
  width: 100%;
  box-shadow: -3px 0px 2px rgba(0, 0, 0, 0.4);
}
.nav {
  background: linear-gradient(to right, #110f5e, #010021);
}
.sticky-header {
  position: fixed;
  z-index: 1000;
  top: 0;
  left: 0;
  width: 100%;
  background: linear-gradient(to right, #110f5e, #010021);
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

@media (max-width: 768px) {
  .navbar,
  .footer,
  .container {
    width: 90%;
    padding: 8px 0px;
  }
}

@media (max-width: 480px) {
  .navbar,
  .footer,
  .container {
    width: 95%;
    padding: 4px 0px;
  }
  section {
    height: auto;
  }
}
</style>
