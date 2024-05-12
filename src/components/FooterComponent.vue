<template>
  <box class="box">
    <div class="image-container">
      <img src="../assets/logo-tagline.png" />
    </div>
    <div class="copyright">
      <p>© 2024 GOVOKASi. All Rights Reserved.</p>
    </div>
    <div class="lokasi">
      <p>
        Jl. Raya Belimbing No.88, Babakan Asem<br />
        Kec. Kosambi, Kabupaten Tangerang,<br />
        Banten 15212
      </p>
    </div>
  </box>
</template>

<style scoped>
.box {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #f0f0f0;
  padding: 20px;
  width: 1516px;
  height: 189px;
}

.image-container {
  align-items: start;
  max-width: 150px;
  height: 130px;
}

.copyright {
  text-align: center;
  align-self: center;
  padding-top: 150px;
}

.lokasi {
  padding-top: 20px;
  text-align: right;
  width: 542px;
  height: 130px;
}
</style>
