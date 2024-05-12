<script></script>

<template>
  <div class="container">
    <div class="row">
      <img src="../assets/logos.png" class="logo-image" />
      <div class="garis">
        <span class="box"></span>
        <h1 class="title">
          DISCOVER YOUR CAREER<span class="title2"> <br />WITH GOVOKASI</span>
        </h1>
      </div>
      <p class="paragraf">
        We are ready to help you find the right career direction according to
        your potential and goals.
      </p>
      <div class="button"><a href="#about" class="link">Learn More</a></div>
    </div>
    <div class="image-container">
      <img src="../assets/HomeImage.png" />
    </div>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  align-items: center;
}
.row {
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
  margin-bottom: 24px;
  font-family: "Bernoru", sans-serif;
}
.title2 {
  color: #ffffff;
  font-family: "Bernoru", sans-serif;
}
.box {
  background-color: transparent;
  border: 5px solid #ffffff;
  margin-right: 24px;
  height: 182px;
}
.paragraf {
  font-size: 12px;
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
}
.garis {
  display: flex;
  align-items: center;
}
.link {
  text-decoration: none;
}
</style>
