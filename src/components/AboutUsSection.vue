<script>
export default {
  methods: {
    openInternLink() {
      window.open('https://bit.ly/GVInternsReg', '_blank');
    },
    openPartnerLink() {
      window.open('https://form.smartsuite.com/swgnyg44/1tg7zwCLDC', '_blank');
    },
  },
};
</script>

<template>
  <div class="aboutsection">
    <div v-motion-slide-visible-left class="about-description">
      <h1 class="title-about-description">
        <span class="box-about-description"></span>About<span
          class="title2-about-description"
        >
          Govokasi</span
        >
      </h1>
      <p class="body-about-description">
        Govokasi is a platform or container for career development for interns
        to find the right internship program and help them realize their full
        potential. Using training and coaching methods to identify, develop, and
        promote their abilities.
      </p>
    </div>
    <div v-motion-slide-visible-right class="about">
      <div class="card">
        <div class="about-content">
          <img
            src="../assets/cooperation.svg"
            alt="about-image"
            style="width: 150px"
          />
          <div>
            <p class="about-link" href="https://wa.me/6281316653083">
              <span class="about-angka">+6000</span> Talent Pool
            </p>
            <p class="about-link" href="mailto:hello@govokasi.com">
              <span class="about-angka">+120</span> Startup Partner
            </p>
            <p class="about-link" href="https://www.instagram.com/govokasi/">
              <span class="about-angka">+80%</span> Intern to Full Time
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.aboutsection {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
}
.aboutsection > *:not(:last-child) {
  margin-right: 20px;
}
.about-description {
  display: flex;
  flex-basis: 55%;
  flex-direction: column;
}

.about-description > *:not(:last-child) {
  margin-bottom: 20px;
}

.title-about-description {
  font-size: 36pt;
  font-weight: bold;
  color: #110f5e;
  margin-bottom: 24px;
}
.title2-about-description {
  color: #fddc58;
}
.box-about-description {
  background-color: transparent;
  border: 5px solid #110f5e;
  margin-right: 24px;
}
.body-about-description {
  text-align: justify;
  font-size: 12pt;
  color: #110f5e;
}

.about {
  flex-basis: 40%;
}
.about-angka {
  font-weight: bold;
  color: #110f5e;
}
.card {
  width: 100%;
  height: max-content;
  padding: 24px;
  background-color: #ffffff;
  display: flex;
  flex-direction: column;
  border-radius: 24px;
  align-items: center;
  box-shadow: 0px 6px 10px 0px rgba(0, 0, 0, 0.2);
}

.about-content {
  width: 100%;
  display: flex;
  align-items: center;
}

@media (max-width: 1024px) {
  .about {
    flex-basis: 40%;
  }
  .about-description {
    flex-basis: 50%;
  }

  .title-about-description {
    font-size: 36px;
    text-align: center;
  }
  .body-about-description {
    font-size: 11pt;
  }
}

@media (max-width: 768px) {
  .aboutsection {
    justify-content: center;
    padding: 120px;
  }
  .aboutsection > *:not(:last-child) {
    margin-right: 0px;
    margin-bottom: 20px;
  }
  .about,
  .about-description {
    flex-basis: 80%;
  }

  .title-about-description {
    font-size: 24px;
    text-align: center;
  }
  .body-about-description {
    font-size: 10pt;
  }
}

@media (max-width: 480px) {
  .about-description {
    flex-basis: 95%;
  }
  .about {
    flex-basis: 95%;
  }

  .title-about-description {
    font-size: 24px;
    text-align: center;
  }
  .body-about-description {
    font-size: 10pt;
  }
}
</style>
