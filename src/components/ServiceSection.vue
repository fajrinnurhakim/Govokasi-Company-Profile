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
  <div class="servicesection">
    <div v-motion-slide-visible-left class="service">
      <p class="paragraf">Three Steps To Success</p>
      <div class="garis">
        <span class="box"></span>
        <h1 class="title">
          BUILDING<span> <br />(PRO)FESIONAL</span>
          <span class="title2"><br />CHARACTER</span>
        </h1>
      </div>
      <p class="paragraf">
        Our interns are continously trained and coached to be the best.
      </p>
    </div>
    <div v-motion-slide-visible-right class="service-card">
      <div class="card">
        <h3 class="card-title">01</h3>
        <h3 class="card-title">IDENTIFY</h3>
        <p class="card-paragraf">
          Register yourself for your dream profession that aligns with the
          skills and abilities you possess, and start building your portfolio.
        </p>
      </div>
      <div class="card">
        <h3 class="card-title">02</h3>
        <h3 class="card-title">DEVELOP</h3>
        <p class="card-paragraf">
          Participate in a 5-7 day project-based internship with real case
          studies and experienced coaches.
        </p>
      </div>
      <div class="card">
        <h3 class="card-title">03</h3>
        <h3 class="card-title">PROMOTE</h3>
        <p class="card-paragraf">
          Qualified talents will be promoted to continue working on projects or
          onboard internships at GOVOKASI’s partner companies.
        </p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.servicesection {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
}
.servicesection > *:not(:last-child) {
  margin-bottom: 20px;
}

.service {
  display: flex;
  flex-basis: 50%;
  flex-direction: column;
  color: #ffffff;
}

.service > *:not(:last-child) {
  margin-bottom: 20px;
}

.title {
  font-size: 30pt;
  font-weight: bold;
  color: #fddc58;
}
.title2 {
  color: #ffffff;
}
.box {
  background-color: transparent;
  border: 5px solid #ffffff;
  margin-right: 24px;
  height: 182px;
}
.garis {
  display: flex;
  align-items: center;
}

.service-card {
  display: flex;
  flex-basis: 50%;
  flex-direction: column;
  color: #ffffff;
}

.service-card > *:not(:last-child) {
  margin-bottom: 20px;
}

.card {
  background-color: #ffffff;
  color: #110f5e;
  padding: 12px;
  border-radius: 12px;
}

.card-title {
  font-size: 24pt;
  color: #110f5e;
}

.card-paragraf {
  font-size: 12pt;
  color: #000000;
}

@media (max-width: 1024px) {
  .servicesection {
    justify-content: center;
  }
  .service {
    flex-basis: 50%;
  }
  .service-card {
    flex-basis: 50%;
  }
  .title {
    font-size: 24pt;
  }
  .box {
    height: 90px;
  }
  .paragraf {
    font-size: 12pt;
  }
}

@media (max-width: 768px) {
  .servicesection {
    justify-content: center;
  }
  .service {
    flex-basis: 80%;
  }
  .service-card {
    flex-basis: 80%;
  }
  .title {
    font-size: 18pt;
  }
  .box {
    height: 90px;
  }
  .paragraf {
    font-size: 11pt;
  }
}

@media (max-width: 480px) {
  .servicesection {
    justify-content: center;
  }
  .service {
    flex-basis: 90%;
  }
  .service-card {
    flex-basis: 90%;
  }
  .title {
    font-size: 16pt;
  }
  .box {
    height: 90px;
  }
  .paragraf {
    font-size: 10pt;
  }
  .card-title {
    font-size: 18pt;
    color: #110f5e;
  }

  .card-paragraf {
    font-size: 10pt;
    color: #000000;
  }
}
</style>
