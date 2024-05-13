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
  <div class="contactsection">
    <div class="register">
      <h1 class="title-register">
        <span class="box-register"></span>Get In<span class="title2-register">
          Touch</span
        >
      </h1>
      <p class="body-register">
        Our objective is to help both interns and companies grow. By helping
        interns find the right internship program to help them realize their
        full potential. During the internship, we provide continuous training &
        coaching to help companies cultivate the interns potential.
      </p>
      <div class="button-container">
        <button @click="openInternLink" class="btn-intern">
          LOOKING FOR INTERSHIP OPPORTUNITY
        </button>
        <button @click="openPartnerLink" class="btn-partner">
          JOIN US AS COMPANY PARTNERS
        </button>
      </div>
    </div>
    <div class="contact">
      <div class="card">
        <h1 class="title-contact">
          <span class="box-contact"></span>Contact<span class="title2-contact">
            Us</span
          >
        </h1>
        <div class="contact-content">
          <a class="contact-link" href="https://wa.me/6281316653083">
            <span><img src="../assets/whatsapp.svg" alt="image-contact" /></span
            >+62 8131 6653 083
          </a>
          <a class="contact-link" href="mailto:hello@govokasi.com">
            <span><img src="../assets/email.svg" alt="image-contact" /></span
            >hello@govokasi.com
          </a>
          <a class="contact-link" href="https://www.instagram.com/govokasi/">
            <span
              ><img src="../assets/instagram.svg" alt="image-contact" /></span
            >@govokasi
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.contactsection {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
}
.contactsection > *:not(:last-child) {
  margin-right: 20px;
}
.register {
  display: flex;
  flex-basis: 55%;
  flex-direction: column;
}

.register > *:not(:last-child) {
  margin-bottom: 20px;
}

.title-register {
  font-size: 36pt;
  font-weight: bold;
  color: #ffffff;
  margin-bottom: 24px;
}
.title2-register {
  color: #fddc58;
}
.box-register {
  background-color: transparent;
  border: 5px solid #ffffff;
  margin-right: 24px;
}
.body-register {
  text-align: justify;
  font-size: 12pt;
  color: #ffffff;
}

.button-container {
  display: flex;
}

.button-container > *:not(:last-child) {
  margin-right: 24px;
}

.btn-intern {
  padding: 12px;
  border-radius: 12px;
  background-color: #fddc58;
  color: #000000;
  border: none;
  cursor: pointer;
  transition: transform 1s ease, background-color 1s ease;
}
.btn-intern:hover {
  background-color: #ffcc00;
  transform: scale(1.1);
}

.btn-partner {
  padding: 12px;
  border-radius: 12px;
  border: none;
  cursor: pointer;
  transition: transform 1s ease, background-color 1s ease;
}
.btn-partner:hover {
  background-color: #000000;
  color: #ffffff;
  transform: scale(1.1);
}

.contact {
  flex-basis: 40%;
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
}
.title-contact {
  font-size: 36pt;
  font-weight: bold;
  color: #110f5e;
  margin-bottom: 24px;
  text-align: center;
}
.title2-contact {
  color: #fddc58;
}
.box-contact {
  background-color: transparent;
  border: 5px solid #110f5e;
  margin-right: 24px;
}
.contact-content {
  width: 100%;
  display: flex;
  flex-direction: column;
}
.contact-link {
  display: flex;
  text-decoration: none;
  color: #000000;
}
.contact-link:hover {
  color: #110f5e;
}
.contact-link span {
  margin-right: 24px;
}

@media (max-width: 1024px) {
  .contact {
    flex-basis: 40%;
  }
  .register {
    flex-basis: 50%;
  }
  .title-contact {
    font-size: 36px;
  }
  .title-register {
    font-size: 36px;
    text-align: center;
  }
  .body-register {
    font-size: 11pt;
  }
}

@media (max-width: 768px) {
  .contactsection {
    justify-content: center;
    padding: 120px;
  }
  .contactsection > *:not(:last-child) {
    margin-right: 0px;
    margin-bottom: 20px;
  }
  .contact,
  .register {
    flex-basis: 80%;
  }
  .title-contact {
    font-size: 24px;
  }
  .title-register {
    font-size: 24px;
    text-align: center;
  }
  .body-register {
    font-size: 10pt;
  }
}

@media (max-width: 480px) {
  .register {
    flex-basis: 95%;
  }
  .contact {
    flex-basis: 95%;
  }
  .title-contact {
    font-size: 24px;
  }
  .title-register {
    font-size: 24px;
    text-align: center;
  }
  .body-register {
    font-size: 10pt;
  }
}
</style>
