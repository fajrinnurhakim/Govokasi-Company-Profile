<template>
  <box class="box">
    <div class="image-container">
      <img class="image-logo" src="../assets/logo-tagline.png" />
    </div>
    <div class="lokasi">
      <p>
        Jl. Raya Belimbing No.88, Babakan Asem Kec. Kosambi, Kabupaten
        Tangerang, Banten 15212
      </p>
    </div>
  </box>
  <box class="box2">
    <div class="copyright">
      <p>© 2024 GOVOKASI. All Rights Reserved.</p>
    </div>
  </box>
</template>

<style scoped>
.box {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #ffffff;
  padding: 20px;
}

.image-container {
  display: flex;
  justify-content: start;
  align-items: center;
  width: 70%;
}
.image-logo {
  width: 40%;
}

.copyright {
  text-align: center;
  align-self: center;
  font-size: 12pt;
  background-color: #ffffff;
  padding: 12px 0px;
}

.lokasi {
  text-align: right;
  font-size: 12pt;
  width: 30%;
}

@media (max-width: 1024px) {
  .lokasi {
    font-size: 12pt;
    width: 50%;
  }
  .copyright {
    font-size: 12pt;
  }
  .image-container {
    width: 70%;
  }
  .image-logo {
    width: 60%;
  }
}

@media (max-width: 768px) {
  .lokasi {
    font-size: 11pt;
    width: 40%;
  }
  .copyright {
    font-size: 11pt;
  }
  .image-container {
    width: 50%;
  }
  .image-logo {
    width: 70%;
  }
}

@media (max-width: 480px) {
  .box {
    flex-direction: column;
  }
  .box2 {
    background-color: white;
  }
  .lokasi {
    font-size: 10pt;
    width: 80%;
    text-align: center;
  }
  .copyright {
    font-size: 10pt;
  }
  .image-container {
    width: 40%;
    padding-bottom: 12px;
  }
  .image-logo {
    width: 100%;
  }
}
</style>
