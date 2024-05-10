<template>
  <div class="navigation">
    <img src="/logo.png" alt="logo" class="logo" /><img />
    <ul class="menu" :class="{ aktif: isMenuActive }">
      <li><a href="#home">Home</a></li>
      <li><a href="#service">Service</a></li>
      <li><a href="#company">Company</a></li>
      <li><a href="#about">About us</a></li>
    </ul>
    <div class="button" @click="toggleMenu">&#9776;</div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isMenuActive: false,
    };
  },
  methods: {
    toggleMenu() {
      this.isMenuActive = !this.isMenuActive;
    },
  },
};
</script>

<style scoped>
.logo {
  width: 120px;
}
.navigation {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.button {
  display: none;
  color: black;
  font-size: 14pt;
}

.button:hover {
  cursor: pointer;
}

.menu {
  margin: 0;
  display: flex;
  list-style: none;
  padding: 0;
}

.menu li {
  padding-left: 0;
  margin-right: 10px;
}

.menu li a {
  padding: 10px;
  color: black;
  text-decoration: none;
  display: inline-block;
}

.menu li a:hover {
  color: blue;
}

@media screen and (max-width: 768px) {
  .menu {
    display: none;
  }

  .menu.aktif {
    display: inline-block;
    position: absolute;
    top: 50px;
    background: rgba(247, 247, 247, 1);
    padding: 10px 20px;
    right: 0;
    left: 0;
  }

  .menu.aktif li a {
    padding: 10px;
    display: inline-block !important;
  }

  .button {
    display: block;
  }
}
</style>
