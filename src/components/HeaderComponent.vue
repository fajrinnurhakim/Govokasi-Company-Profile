<template>
  <div class="navigation">
    <img src="/logo.png" alt="logo" class="logo" /><img />
    <ul class="menu" :class="{ aktif: isMenuActive }">
      <li><a href="#home">Home</a></li>
      <li><a href="#about">About us</a></li>
      <li><a href="#service">Our Service</a></li>
      <li><a href="#company">Company Values</a></li>
      <li><a href="#contact">Contact Us</a></li>
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
  z-index: 99;
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
  font-size: 12pt;
}

.menu li {
  padding-left: 0;
}

.menu li a {
  padding: 10px;
  color: black;
  text-decoration: none;
  display: inline-block;
  padding: 12px;
  transition: background-color 1s ease;
  border-radius: 12px;
}

.menu li a:hover {
  color: #110f5e;
  background-color: #fddc58;
}

@media screen and (max-width: 768px) {
  .menu {
    display: none;
  }
  .button {
    padding: 6px;
    border-radius: 6px;
    color: #000000;
    transition: background-color ease-in-out 2s;
  }
  .button:hover {
    padding: 6px;
    background-color: #110f5e;
    border-radius: 6px;
    color: #ffffff;
  }
  .menu.aktif {
    display: block;
    position: absolute;
    top: 55px;
    background: #ffffff;
    right: 0;
    left: 0;
    text-align: center;
    transition: opacity 2s ease, top 2s ease-in-out;
    opacity: 1;
  }

  .menu.aktif li a {
    display: block;
  }
  .menu.aktif li a {
    border-radius: 0px;
  }

  .button {
    display: block;
  }
}
</style>
