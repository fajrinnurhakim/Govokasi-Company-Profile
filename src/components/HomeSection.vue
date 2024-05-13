<script></script>

<template>
  <div class="container">
    <div class="row">
      <img src="../assets/logos.png" class="logo-image" />
      <div class="garis">
        <span class="box"></span>
        <h1 class="title">
          BUILD YOUR DREAM CAREER<span class="title2">
            <br />WITH GOVOKASI</span
          >
        </h1>
      </div>
      <p class="paragraf">
        We are ready to help you find the right career direction according to
        your potential and goals.
      </p>
      <div class="button"><a href="#about" class="link">Learn More</a></div>
    </div>
    <div class="image-container">
      <img class="image-content" src="../assets/home-image.svg" />
    </div>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  align-items: center;
}
.row {
  width: 50%;
  display: flex;
  flex-direction: column;
}
.row > *:not(:last-child) {
  margin-bottom: 20px;
}
.logo-image {
  height: 50px;
  width: 250px;
}
.title {
  font-size: 30pt;
  font-weight: bold;
  color: #fddc58;
  font-family: 'Bernoru', sans-serif;
}
.title2 {
  color: #ffffff;
  font-family: 'Bernoru', sans-serif;
}
.box {
  background-color: transparent;
  border: 5px solid #ffffff;
  margin-right: 24px;
  height: 182px;
}
.paragraf {
  font-size: 12pt;
  color: white;
}
.button {
  padding: 12px;
  border-radius: 12px;
  border: none;
  cursor: pointer;
  transition: transform 1s ease, background-color 1s ease;
  width: 175px;
  height: 52px;
  text-align: center;
  background-color: #fddc58;
  color: #110f5e;
}
.button:hover {
  transform: scale(1.1);
  background-color: #ffcc00;
}
.garis {
  display: flex;
  align-items: center;
}
.link {
  text-decoration: none;
}
.image-container {
  width: 50%;
  height: auto;
}
.image-content {
  width: 100%;
}

@media (max-width: 1024px) {
  .container {
    display: flex;
    align-items: center;
  }
  .logo-image {
    height: auto;
    width: 200px;
  }
  .title {
    font-size: 18pt;
  }
  .box {
    height: 120px;
  }
  .paragraf {
    font-size: 12pt;
  }
}

@media (max-width: 768px) {
  .container {
    display: flex;
    align-items: center;
  }
  .logo-image {
    height: auto;
    width: 150px;
  }
  .title {
    font-size: 16pt;
  }
  .box {
    height: 90px;
  }
  .paragraf {
    font-size: 11pt;
  }
}

@media (max-width: 480px) {
  .container {
    display: flex;
    flex-direction: column-reverse;
  }
  .row {
    width: 95%;
    align-items: center;
  }
  .logo-image {
    display: none;
  }
  .title {
    font-size: 16pt;
    text-align: center;
  }
  .box {
    display: none;
  }
  .paragraf {
    font-size: 10pt;
    text-align: center;
  }
  .button {
    margin-bottom: 24px;
  }
}
</style>
